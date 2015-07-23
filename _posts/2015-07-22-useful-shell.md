---
author: leon
comments: true
date: 2014-01-21 10:37:25+00:00
layout: post
title: '[Beaglebone] 个人常用Shell集锦' 
categories:
- Shell

tags:
- Shell
---

shell是Unix系统的一个特色，fuck点和hack点并存：

- fuck点： 需要记住一些复杂的命令，看组织得还算不错的man & help，有一个学习的过程，相比所见所得的视窗真是反人类。代表包括grep、sed、awk。
- hack点： 可以用简单的命令完成复杂的工作，如替换多个文档里的字符串，grep、seed、find再结合正则表达式简直无敌，代表包括grep、sed、awk。

本文将平时用的一些shell集合起来，待不时之需。

### 文本替换

1. 替换所有特定后缀的文件中的字符串，无正则 

    ```bash
    find -type f -name "*.markdown" | xargs sed -i 's/${oldstr}/${newstr}/g'
    ```

### awk
1. awk工作模式
    awk被设计成数据流方式处理，内建很多基本的语法，因此使用起来非常灵活和强大，常用作字符处理。最基本的awk命令模式类似：

    `awk ' BEGIN{  print "start" } pattern { commands } END{ print "end" }  file`
    
    > How it Works? The awk command works in the following manner:
    > 
    > - Execute the statements in the BEGIN { commands } block.
    > - Read one line from the file or stdin, and execute pattern { commands }. Repeat this step until the end of the file is reached.
    > - When the end of the input stream is reached, execute the END { commands } block.

    awk首先调用BEGIN区块，然后逐行处理流，按照相应的匹配模式作相应的处理动作，最后调用END区块。 一个简单的行数计数用法如下：

    `awk 'BEGIN {i=0} {i++} END {print i}' filename`

2. 特殊变量

    |Name|    Usage|
    |----|---------|
    |NR  |It stands for number of records and corresponds to current line number under execution.|
    |$0  |It is a variable that contain the text content of current line under execution.        |
    |$1  |It is a variable that holds the text of the first field.                               |
    |$2  |It is the variable that holds the test of the second field text.
    |NF  |It stands for number of fields and corresponds to number of fields in the current line under execution (Fields are delimited by space).|



### Git

1. git恢复已经删除的文件

直接从本地把文件checkout出来就可以了，用不着从远程服务器上pull下来，因为，所有的历史版本你的本地都有的。 
具体做法 `git checkout file` 同时恢复多个被删除的文件：`git ls-files -d | xargs -i git checkout {}`

在使用Git的过程中，有时可能会有一些误操作 比如：执行`checkout -f` 或 `reset -hard` 或 `branch -d`删除一个分支 结果造成本地（远程）的分支或某些commit丢失 可以通过reflog来进行恢复，前提是丢失的分支或commit信息没有被`git gc`清除 一般情况下，gc对那些无用的object会保留很长时间后才清除的 reflog是git提供的一个内部工具，用于记录对git仓库进行的各种操作,可以使用`git reflog show`或`git log -g`命令来看到所有的操作日志。恢复的过程很简单：通过`git log -g`命令来找到我们需要恢复的信息对应的`commit_id`，可以通过提交的时间和日期来辨别。

一个好的办法是运行：

1. `git log –since="2 weeks ago" – myfile` 可以2个星期期间的myfile历史；
2. `git log –branches="develop"` 可以查看develop的commit 
3. 通过`git branch recover_branch[新分支] commit_id`来建立一个新的分支

这样，我们就把丢失的东西给恢复到了`recover_branch`分支上了。

**Q1:** 如果是不小心执行了`git reset`，还有办法取消吗？ 

**A1:** `git reflog` 查看操作历史，找到之前 HEAD 的 hash 值，然后 `git reset –hard` 到那个 hash 即可。

**Q2:** 怎样找回历史版本中删除的文件？

**A2:** 先确定需要恢复的文件要恢复成哪一个历史版本(commit)，假设那个版本号是： `commit_id`，那么`git checkout [commit_id] – <path_to_file>` 就可以恢复


### Diff & Patch

1. diff

    ```bash
    cd your-kernel-tree
    cd ..
    diff -Narup org-kernel-source your-kernel-tree > kernel.patch
    ```
-x 过滤掉所比较目录中一些不想比较的文件类型，可以使用其他的pattern。实际上如果需要过滤的文件类型比较多的时候，使用-x这个选项就有点麻烦了，查看了文档之后，diff提供了更加方便的参数过滤文件。 -X excludefile 忽略在excludefile中的文件类型，注意每种文件占一行 pallying patches

2. patch

    ```bash
    cd kernel-source
    patch -p1 < ../kernel.patch
    patch -R -p1 < ../kernel.patch
    ```
    
