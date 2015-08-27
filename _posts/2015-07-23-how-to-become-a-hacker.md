---
author: leon
comments: true
date: 2015-07-23 19:10:25+00:00
layout: post
title: '[搬运] 如何成为一名黑客' 
categories:
- 计算机文化
- 搬运

tags:
- 计算机文化
---

原文文档：[http://catb.org/~esr/faqs/hacker-howto.html](http://catb.org/~esr/faqs/hacker-howto.html)

###为什么会有这份文档？

作为 [http://www.catb.org/jargon Jargon File]（译注：黑客行话大全）的编辑和几份其他类似性质知名文章的作者，我经常收到充满热情的网络新手的电子邮件询问：“我如何才能成为一名出色的 Hacker？”早在 1996 年，我注意到网上似乎没有任何的 FAQ 或者 Web 形式的文档提到及这个至关重要的问题，因此我写了这份文档。现在，很多 Hacker 都认为这是一篇权威性文档，那我也姑且这么认为吧。不过，我不认为我是这个话题的绝对权威；如果你不喜欢这篇文档，你也可以自己写一份。

如果你读到的是这份文档的离线拷贝，你可以在 http://catb.org/~esr/faqs/hacker-howto.html 读到最新版本。

注意：文档的结尾有一份 [http://translations.readthedocs.org/en/latest/hacker_howto.html#faq FAQ（常见问题解答）]。如果你想通过邮件询问我关于这份文档的问题，请先读这份 FAQ 看看能否找到答案——一遍不行就读两遍。

目前这份文档有很多翻译版本：

- [http://www.slashproc.net/doc/howto-ar.html 阿拉伯语]
- [http://moneyaisle.com/worldwide/how-to-become-a-hacker-be 白俄罗斯语]
- [http://www.olemichaelsen.dk/hacker-howto.html 丹麦语]
- [http://www.knudde.be/index.php?page_name=hacker_howto 荷兰语] 
- [http://www.kakupesa.net/hacker 爱沙尼亚语]
- [http://www.linuxtaskforce.de/hacker-howto-ger.html 德语]
- [http://users.otenet.gr/%7Eindy90/hacker-howto-gr/ 希腊语]
- [http://www.victorfleur.com/documents/hacker.html 意大利语] 
- [http://he.wikisource.org/wiki/%D7%90%D7%99%D7%9A_%D7%9C%D7%94%D7%99%D7%95%D7%AA_%D7%94%D7%90%D7%A7%D7%A8 希伯来语]
-  [http://stian.atlantiscrew.net/doc/hacker-howto.html 挪威语] 
- [http://jvdm.sdf1.org/pt/raquer-howto/ 葡萄牙语（巴西）]
- [http://garaj.xhost.ro/hacker-howto/hacker-howto.ro.htm 罗马尼亚语] 
- [http://www.sindominio.net/biblioweb/telematica/hacker-como.html 西班牙语]
- [http://www.belgeler.org/howto/hacker-howto/hacker-howto.html 土耳其语]
- [http://www1.tripnet.se/%7Emly/open/faqs/hacker-howto.se.html 瑞典语] 

注意由于这份文档时有修正，所以以上翻译版本可能有不同程度的过时。

装饰本文的“五点九宫格”图像被称作“glider”，在一种叫做[http://dmoz.org/Computers/Artificial_Life/Cellular_Automata/ Life]的数学模型中，这个简单的样本有一些异乎寻常的属性，多年以来 Hacker 们都为此着迷。我认为这个图像是一个很好的黑客徽标：它显得抽象而且神秘，而且像是一扇大门，通向一个截然不同的有其内在逻辑的世界。你可以阅读更多关于[http://www.catb.org/~esr/hacker-emblem/ Glider 徽标] 的内容。


###什么是黑客？

[http://www.catb.org/jargon Jargon File]讲了一堆关于“hacker”这个词的定义，大部分是关于“技术高超”、“热衷解决问题”、以及“超越极限”的内容。但如果你只想知道如何成为一名黑客的话，真正重要的只有两条。

这可以追溯到几十年前，那时候第一代分时微型计算机才刚刚诞生, 而 ARPAnet 的实验也才刚展开。那时的编程专家和组网高手建立了一个具有共享性质的文化社群， “hacker” 这个名词就是其中的成员创造的。黑客们建立了互联网，黑客们让 Unix 操作系统演化到现在的模样，黑客们经营着 Usenet，黑客们让万维网运转起来。如果你是这个文化的一部分，如果你对这种文化有所贡献，而且这个社群的其它成员也认识你并称你为 hacker，那么你就是一名黑客。

黑客的思维方式并不仅仅局限在软件黑客的文化圈内。也有人用黑客态度对待其它事情，如电子和音乐方面——其实你可以在任何最高级别的科学和艺术活动中发现它的身影。软件黑客对这些领域的践行者尊重有加，并把他们也称作黑客——有人宣称黑客天性是绝对独立于他们工作的特定领域的。但在这份文档中，我们将集中书写在软件黑客的技术和态度，以及发明了“黑客”一词的、以共享为特征的文化传统。

有另外一群人大声嚷嚷着自己是黑客，但他们根本不是。他们主要由青少年男性构成，是一些蓄意破坏计算机和电话系统的人。真正的黑客把这些人叫做“骇客”(cracker)，并不屑与之为伍。黑客们通常认为他们是一群懒散、没有责任心、而且不是很聪明的人。会通过热接线发动汽车并不意味着你是一个汽车工程师。一样的道理，会破坏安全也不意味着你是一名黑客，不幸的是，很多记者和作家往往错把“骇客”当成黑客；这种做法一直使真正的黑客感到恼火。

根本的区别是：黑客搞建设，骇客搞破坏。

如果你想成为一名黑客，请接着读下去。如果你想做一个骇客，就去读 alt.2600 新闻组吧，顺便准备好去蹲个五到十年的监狱，而且最终你会意识到你并不像自己想象的那么聪明。

关于骇客，我能说的只有这些。


###黑客的态度

黑客们解决问题，建设事物，同时他们信仰自由和无私的双向帮助。要想作为一名黑客被社群认同，你需要体现出自己已经具备了这种态度。而要体现出这种态度，你就得真正相信和赞同这种态度。

但是，如果你认为培养黑客态度只是进入黑客文化圈的敲门砖，那就大错特错了。这种态度将有助于有助于你的学习，并且能为你提供源源不断的动力，所以它对你而言是至关重要的。和所有创造性的艺术一样，成为大师的最有效方法，就是模仿大师的精神——智力上的模仿还不够，还要从感情上进行模仿。

 或者正如下面这首现代的禅诗讲的：
 修行之道：
 关注大师的言行，
 跟随大师的举动，
 和大师一并修行，
 领会大师的意境，
 成为真正的大师。

所以，如果你想成为一名黑客，反复读下面的事情直至你相信它们为止：


####这个世界充满了令人着迷的问题等着我们解决

做一名黑客会有很多乐趣，但是这些乐趣需要付出很多努力才能获得。这些努力需要动力。成功的运动员在表演和超越自我极限的时候获得身体上的愉悦，并把这种愉悦作为自己的动力。同样，为了成为一名黑客，你要从解决问题、磨练技术，以及锻炼智力中得到基本的享受。

如果你不是天性如此，而你又想成为一名黑客，你就要设法成为这样的人。否则你会发现，你的黑客热情会被其他分心的事物吞噬掉——如金钱、性、以及社交圈的认同。

（你必须建立对于自己学习能力的信念——就算你掌握的知识不足以解决当前的问题，如果你从问题的一小部分下手并从中学习，你将学到足够的知识用来解决下一部分——以此类推，直到整个问题都被你解决为止。）


####一个问题不应该被解决两次

有创新能力的大脑是一种宝贵的有限资源。当世界还充满非常多有待解决的有趣的新问题时，它们不应该被浪费在重新发明轮子的事情上。

作为一名黑客，你必须相信其他黑客的思考时间是宝贵的——因此共享信息、解决问题、并发布结果给其他黑客几乎是一种道义，这样其他人就可以去解决新问题，而不用在旧问题上面浪费精力了。

（这并不是在说你有义务把自己所有的作品都免费发布出来，但这样做的黑客能获得大家最大的尊敬。使用黑客技能养家糊口甚至发财致富都没关系，只要你别忘记自己作为一个黑客的责任，不背离黑客群体即可。）


####无聊和乏味的工作是罪恶

黑客（以及所有创造力的人们）都不应该被愚蠢的重复性劳动所困扰。重复性劳动浪费了他们解决新问题的时间，而解决新问题正是黑客最大的价值所在。这种浪费会伤害到每一个人。无聊和乏味的工作不仅仅是令人不舒服而已，而且本身就是一种罪恶。

作为一个黑客，你必须坚信这点并尽可能多地将乏味的工作自动化，这不仅是为了你自己，也是为了其他人（尤其是其他黑客们）。

(对此有一个明显的例外。黑客有时为了休息大脑、学习技能、或者别的特别的原因，也会做一些在他人看来是重复性或枯燥的事情。但这是自愿的——只要是有思维能力的人，就不应该被迫做无聊的活儿。）


####崇尚自由

黑客们是天生的反权威主义者。任何能向你发号施令的人都可以让你停止解决令你着迷的问题，同时，按照权威主义者的一般思路，他通常会给出一些极端愚昧的理由。因此，不论何处，任何权威主义的做法，只要它影响到了你和其他的黑客，你就要和它斗到底。

（这并非向所有权威挑战。儿童需要监护，罪犯要被看管起来。如果服从命令得到某种东西比起用其他方式得到它更节约时间，黑客可以同意接受某种形式的权威。但这是一个有限度的，斟酌过的的交易；那种权威主义者想要的个人服从是不在考虑范围内的。）

权威主义者喜欢审查和保密。他们不信任自愿的合作和信息的共享——他们只喜欢由他们控制的所谓“合作”。因此，作为一个黑客，你应该对审查、保密，以及使用武力或欺骗去压迫有行为能力的人们的做法有一种本能的敌意。同时你要有为此信念付出的意愿。


####态度不能替代能力

作为一名黑客，你必须培养起这些态度。但只具备这些态度并不能使你成为一名黑客，也不能使你成为一个运动健将和摇滚明星。成为一名黑客需要智力、实践、奉献精神、以及辛苦的工作。

因此，你必须学着忽略态度问题，并尊重各种各样的能力。黑客们不会为那些装模做样的人浪费时间，但他们却非常尊重能力——尤其是从事黑客工作的能力（虽然有能力总归是好事）。如果能具备少有人能掌握的技能就更好了，当然如果你具备一些急需的技能，而这些技能又需要敏锐的思维、高超的技巧、和专注的精神，那就是再好不过了。

如果你尊重能力，你就会享受到提高自己能力的乐趣——辛苦的工作和奉献将不会是一件苦差事，而是一种紧张的娱乐，这是成为黑客至关重要重要的一点。


###黑客的基本技能

黑客态度重要，但技术更加重要。态度无法替代技术，在你被别的黑客称为黑客之前，你必须掌握一些基本的技术作为你随身携带的工具。

随着新技术的出现和老技术的过时，这个工具包的内容也在不断改变。比如以前机器语言编程也被列在里边，而 HTML 是直到最近才包括进去的。不过现在可以清楚地告诉你包含以下内容：


####学习如何编程

这一条无须多说，当然是最基本的黑客技能。如果你还不会任何编程语言，我建议你从 Python 开始学起。它设计清晰，文档齐全，而且对初学者比较友好。虽然它很适合作为一种入门语言，但它不仅仅只是个玩具；它非常强大、灵活，也适合做大型项目。我在一篇更详细的[http://www.linuxjournal.com/article.php?sid=3882 Evaluation of Python]（译注：Python 试用体验）中有更详细的论述。[http://docs.python.org/tutorial/ Python 网站]有很好的[http://sebug.net/paper/python/ 入门教程]。

我曾经推荐过将 Java 作为初学的语言，但[http://www.crosstalkonline.org/storage/issue-archives/2008/200801/200801-Dewar.pdf 这则批评]改变了我的想法（在里边搜索”The Pitfalls of Java as a First Programming Language” 就知道我的意思了）。作为一名黑客，你不能像人们挖苦的一样，“像水管工人一样装电脑”，你必须知道各个部件的工作原理。现在我觉得可能还是学过 C 和 Lisp 后再学 Java 比较好。

有一个大体的规律，就是如果你过于偏重使用一种语言，这种语言一方面会成为你得心应手的工具，另一方面也会阻碍你的学习。有这个问题的不只是编程语言，类似 RubyOnRails、CakePHP、以及 Django 的 web 应用框架也有这个问题，它们只会让你肤浅地懂得一些东西，当你碰到难以解决的问题或者需要调试时，你就可能不知所措了。

如果你想进入正式的编程领域，你将不得不学习 C 语言，它是 Unix 的核心语言。C++ 与 C 非常其他类似；如果你了解其中一种，学习另一种应该不难。但这两种都不适合编程入门者学习。而且事实上，你越避免用C编程，你的工作效率会越高。

C 语言效率极高，而且占用很少的系统资源。不幸的是，C 的高效是通过你手动做很多底层的管理（如内存管理）来达到的。底层代码都很复杂，而且极易出现 bug，你要花很多的时间调试。而现今的计算机速度如此之快，花时间调试程序通常是得不偿失——比较明智的做法是使用一种运行较慢、效率较低，但能大幅节省你的开发时间的语言。因此，还是选择 Python 吧。

其他对黑客而言比较重要的语言包括 Perl 和 LISP。从实用的角度来说，Perl 是值得一学的；它被广泛用于动态网页和系统管理中，因此，即便你从不用Perl 写程序，至少也应该学会读懂 Perl。许多人使用 Perl 的理由和 我建议你使用 Python 的理由一样，都是为了避免用 C 完成那些不需要 C 高效率的工作。你会需要理解那些工作的代码的。

LISP 值得学习的理由不同——最终掌握了它时你会得到丰富的启迪和经验。虽然你实际上很少会用到 LISP，但这些经验会使你在以后的日子里成为一个更好的程序员。

当然，实际上你最好五种都会（Python，Java，C/C++，Perl 和 LISP）。除了是最重要的黑客语言外，它们还代表了截然不同的编程思路和方法，每种都会让你受益非浅。（你可以通过修改 Emacs 编辑器的模式）

单单学习编程语言并不会让你达到黑客的程度，甚至连程序员的程度都难企及——你需要脱离某种编程语言的素服，学习通过编程解决问题的思路。要成为一个真正的黑客，你需要达到几天就能学会一门编程语言的水平，你可以将文档里的信息和你已经掌握的知识结合起来，很快就学会一门编程语言。这意味着你需要先学会机种思路截然不同的语言才行。

编程是一个复杂的技能，我无法给你完整的指南来教会你如何编程，不过我可以告诉你，书本和课程也无法教会你如何编程——很多黑客，或者也许几乎所有的黑客，都是靠自学的。你从书本上学到语言的特点——只是一些皮毛，但要使书面知识成为自身技能，你只能通过实践和虚心向他人学习。因此你要做的就是 (a) 读代码，(b) 写代码。

Peter Novig 是 Google 公司的顶尖黑客之一，而且是最受欢迎的 AI 课本的一名作者。他写了一篇好文章名叫[http://norvig.com/21-days.html Teach Yourself Programming in Ten Years]（译注：十年教会自己编程），其中的“recipe for programming success”（译注：编程的成功之道）尤其值得一读。

学习编程就象学习自然语言写作一样。最好的做法是读一些大师的名著，试着自己写点东西，再读些，再写点，再读些，再写点……如此往复，直到你的文章具备范文的力量和感觉为止。

以前要找适合阅读的好代码并不容易，因为几乎没有大型程序的源代码能让新手练手。这种状况已经戏剧性地发生变化；开源软件、编程工具、和操作系统（全都由黑客写成）现在已经随处可见。让我们在下一个话题中继续讨论……


####学习使用开源的 Unix 系统

我将假设你已经有一台个人计算机供自己使用了（你可以体会一下这意味着多少东西。早些时候，计算机是如此的昂贵，没有人能买得起。而黑客文化就是在那样的环境下演化来的）。新手们能够朝学习黑客技能迈出的最基本的一步，就是找一版 Linux 或 BSD-Unix，安装在个人电脑上，并且把它跑起来。

没错，这世界上除了Unix还有其他操作系统。但它们都是以二进制形式发布的——你无法读到它的源代码，也不可能修改它。尝试在运行 DOS、Windows、或 MacOS 的机器上学习黑客技术，就象是穿着骑士铠甲学跳舞。

除此之外，Unix 还是 Internet 的操作系统。你可以学会上网却不知道 Unix，但你不了解 Unix 就无法成为一名 Internet 黑客。因此，今天的黑客文化在很大程度上是以 Unix 为核心的。（这点并不总是真的，一些很早的黑客对此一直很不满，但 Unix 和 Internet 之间的联系已是如此之强，就连 Microsoft 这样强力的公司也对此也无可奈何。）

所以, 安装一套 Unix 吧——我个人偏爱 Linux，但还有其他种类共你选择（是的，你可以在同一电脑上同时安装 Linux 和 DOS/Windows)。学习它，运行它，鼓捣它。用它上 Internet。阅读它的源代码。修改它的源代码。你会用到很多优秀的编程工具（包括 C， LISP，Python 及 Perl），这些工具在 Windows 下是做梦都没法得到的。你会觉得乐趣无穷。当你有一天成为大师再回顾初学的日子，你会觉得那时学到的东西可真多。

如果你想了解更多关于学习 Unix 的信息，读一下 The Loginataka（译注：ESR 的另一著作，可以称为黑客大藏经）吧。也许你还想看看 The Art of Unix Programming （译注：Unix 编程艺术，经典著作）。

你可以访问 Linux Online! 网站，这个网站可以帮你起步。你可以从那里下载到Linux，或者更好的办法是找一个本地的 Linux 用户组，让他们帮你安装 Linux。

在这份 HOWTO 文档发布后的前十年里，关于 Linux 我写的是，从新人的观点来看，所有的Linux 发行版都差不多，但在 2006-2007 之间，我们终于有了一个最佳选择： Ubuntu。我们可以说各种Linux 发行版各有千秋，但 Ubuntu 是新人最容易上手的一个发行版。

你可以在 www.bsd.org 找到 BSD Unix 的求助及其他资源。

Linux 有一种被称为 Live CD 的发行方式，这种发行版会从CD 运行起来，而且不会动到你硬盘里的东西，Live CD 是尝试 Linux 的一个不错的方法。由于光驱读写本来就比较慢，Live CD 的速度一般也会比较慢，不过 Live CD 总归是一个能尝试各种可能性而又不过激的方法。

我有写一篇关于 Unix 和 Internet 基础的入门文章。

对于新手，我以前不鼓励你自己独立安装Linux 或者 BSD，现在这些系统的安装工具已经足够好了，就算对新手来说，独立安装操作系统也不是不可能的事。无论如何，我还是推荐你联系本地的 Linux 用户组，向他们寻求帮助，这会进程更加顺利。


####学会使用万维网以及编写 HTML

黑客文化建造的大多东西都在你看不见的地方发挥着作用。浙西东西可以帮助工厂、办公室、以及大学正常运转起来，但从表面上很难看到它们对非黑客的普通人的生活的影响。而 Web 是一个大大的例外。就连政客也同意，这个庞大耀眼的黑客玩具正在改变整个世界。就算只是因为这个（还有许多其它的原因），Web 也值得你一学。

这并不是仅仅意味着如何使用浏览器（谁都会），而是要学会如何写 HTML，也就是 Web 的标记语言。如果你不会编程，写HTML会教你一些有助于学习的思考习惯。因此，先完成一个主页。（网上有很多不错的资源，比如 [http://htmldog.com/ 这个 HTML 入门教程]。)

但仅仅拥有一个主页不能使你成为一名黑客。 Web里充满了各种网页。大多数是毫无意义的、毫无信息量的垃圾——界面时髦的垃圾，不过还是垃圾（更多相关信息访问[http://catb.org/~esr/html-hell.html The HTML Hell Page]）。

要想有价值，你的网页必须有内容——它必须有趣或对其它黑客有帮助。这是下一个话题所涉及的……


####学习英语，如果你的水平不够用的话

作为一个以英语为母语的美国人，我以前很不情愿提到这点，免得被当做一种文化上的帝国主义。但相当多以其他语言为母语的人一直劝我指出这一点，那就是：英语是黑客文化和 Internet 的工作语言，只有懂英语，你才能在黑客社区顺利做事。

大概1991年的时候，我就了解到许多黑客在技术讨论中使用英语，甚至有时他们来自同一种母语也在用英文讨论。在现阶段，英语有着比其他语言丰富得多的技术词汇，因此是一个对于工作来说相当好的工具。基于类似的原因，英文技术书籍的翻译通常都不怎么令人满意。（如果有翻译的话）。

Linus Torvalds 是芬兰人，但他的代码注解是用英语写的（很明显他从没想过其他的可能性）。他流利的英语。是他能够管理全球范围的 Linux 开发人员社区的重要因素。 这是一个值得学习的例子。

就算你的母语是英语，这也无法保证你的语言技能足够达到黑客的标准。如果你的写作文字不通、语法混乱、错字连篇，包括我在内的大部分的黑客都会忽略你的存在。虽然写作马虎不一定意味着思考也马虎，但我们发现两者的关联性还是挺强的——马虎的头脑对我们来说毫无价值，如果你写作能力不够，就好好学习写作吧。


###提高自己在黑客圈中的地位

和大部分不涉及金钱的文化一样，黑客王国靠声誉运转。你设法解决有趣的问题，但它们到底多有趣，你的解法有多好，是要由那些和你具有同样技术水平，或比你更厉害的人去评判的。

相应地你需要认识到，当你在玩黑客游戏时，你的分数主要是靠其他黑客对你的技术的评价得到的（这就是为什么只有在其它黑客称你为黑客时，你才算得上是一名黑客）。常人的印象里，黑客是一项独来独往的工作，所以上述评价方式并不为众人所知。另一个黑客文化误区是拒绝承认自我或外部评价是一个人的动力，这种想法在 1990 年代末以后就逐渐衰退了，但现在还有人这么认为。这也是让上述评价方式鲜为人知的原因之一。

明确地讲，黑客行为就是人类学家所称的“奉献文化”。在这里你不是凭借你对别人的统治来建立地位和名望，也不是靠美貌，或拥有其他人想要的东西，而是靠你的贡献。尤其是贡献你的时间、你的创造、以及你的技术成果。

要获得其他黑客的尊敬，你可以从下面五种事情着手：


####撰写开源软件

第一个方法（也是最重要，最传统的方法）是写些被其他黑客认为有趣或有用的程序，并把程序源代码提供给整个黑客文化圈使用。

（过去我们称之为“free software （自由软件）”， 但这却使很多不知 free 的精确含义的人感到困惑。现在我们很多人，根据搜索引擎网页内容分析，至少三分之二的人在使用”open-source software，即“开源软件”这个词）。

黑客领域里最受尊敬的偶像，是那些写了大型的、好用的、用途广泛的软件，并把它们发布出来，使得每人都在使用他软件的人。

但是从历史方面来讲有一点值得一提。虽然黑客们一直认为开源软件的开发者是真正的黑客，但在 1990 年代中期以前，大部分黑客会把自己的主要时间用来撰写闭源软件，直到我 1996 年开始写这篇 HOWTO 时也是如此。但从 1997 年后开源软件进入了主流，而且改变了这一切。以现在的观点来看，“黑客社群”和“开源开发者”是对这一个社群的两种称呼，但值得记住的是，以前这两者的概念并不完全一样。要了解更多信息，你可以看看 关于黑客、开源、以及自由软件的历史这一节的内容。


####帮助测试并调试开源软件

黑客也尊敬那些使用和测试开源软件的人。这个世界并不完美，我们不可避免地要把大多数的开发时间放在调试阶段。这就是为什么任何有头脑的开源代码的作者都会告诉你好的 beta 测试员象红宝石一样珍贵。好的测试者知道如何清楚描述出错症状，很好地定位错误，能忍受快速发布中的 bug，并且乐意配合做一些例行的诊断性工作。一个优秀的测试者可以让一场旷日持久辛苦不堪的调试大战变成一场有益身心的小打小闹。

如果你是个新手，试着找一个你感兴趣的正在开发中的程序，做一个好的 beta 测试员。你会自然地从帮着测试，进步到帮着抓 bug，到最后帮着改程序。你会从中学到很多，而且善因种善果，以后别人也会很乐意帮助你。


####发布有用的信息

另一件好事是收集整理有用有趣的信息，做成网页或类似 FAQ 的文档，并且让大家都能看到。

技术性 FAQ 的维护者会受到和开源代码的作者一样多的尊敬。


####帮助维护基础设施的运转

黑客文化（还有互联网工程方面的发展）是靠志愿者推动的。要使Internet能正常工作，就要有大量枯燥的工作不得不去完成——管理邮件列表和新闻组，维护大型软件库，开发 RFC 和其它技术标准等等。

做这类事情的人会得到很多尊敬，因为每人都知道这些事情费时颇多，而又不象编程那样有趣。做这些事情需要奉献精神。


####为黑客文化本身服务

最后，你可以为这个文化本身做宣传（例如像我这样，写一个“如何成为黑客”的教程 :-) ）这并不要求在你已经在这个圈子呆了很久，因以上四点中的某点而出名，有一定声誉后才能去做。

黑客文化没有领袖，这点是确认无疑的。但黑客圈里确实有些文化英雄、部落长者、史学家、还有发言人。如果你在这圈里呆足够长时间，你也许也能成为其中之一。 记住：黑客们不相信他们的部落长者的自夸，因此过分追求这种名誉是危险的。与其奋力追求，不如先摆正自己的位置，等它自己落到你的手中——那时则要做到谦虚和优雅。


###黑客和书呆子(Nerd)的联系

和大家普遍认为的相反，并不是只有书呆子才能成为一名黑客。但它确实有帮助，而且许多黑客事实上是书呆子。做一个深居简出的人有助于你集中精力进行十分重要的事情，如思考和编程。

因此，很多黑客都接受了“geek（奇客）”这个标签，并把它作为骄傲的奖章——这是宣布他们独立于主流社会期望的一种方式（这个标签也是他们喜欢科幻小说和策略型游戏的标记，而这些也是很多黑客喜欢的东西）。1990 年代更多用的称呼是“nerd（书呆子）”，那时“nerd”只带点轻微的贬义，而“geek”则是地地道道的蔑称，而在 2000 年以后，这两者逐渐调转过来了，至少再美国的大众文化中是这样。而到了现在，甚至在非技术人群里，也有不少以 geek 精神为傲的文化团体。

如果你能集中足够的精力做好黑客工作同时还能有正常的生活，这是件好事。现在要做到这一点比我在 1970 年代还是新手的时候要容易的多；如今主流文化对技术怪人要友善得多。甚至有越来越多的人意识到黑客通常是很好的恋人和配偶的材料。

如果你因为生活上不如意而迷上做黑客，那也没什么——至少你不会分神了。也许你以后还能找到自己的生活。


###向黑客的格调靠拢

重申一下，要做一名黑客，你必须深入体验黑客精神。计算你不在计算机边上，你仍然有很多对黑客工作有帮助的事情可做。它们并不能替代真正的编程（没有什么能替代编程），但很多黑客都那么做，并感到它们与黑客的本质存在某些基本的连系。

- 学会用母语流畅地写作。尽管很多人认为程序员写不出好文章，但是有相当数量的黑客（包括所有我知道的最棒的黑客）都是很有能力的写手。
- 阅读科幻小说。参加科幻小说讨论会。（这是一个认识黑客和准黑客的好方法）
- 学习一种武术。武术中需要的精神自律能力和黑客在这方面的需求非常相似。黑中最受欢迎的武术是来自亚洲的空手格斗类武术，例如跆拳道、空手道、武术、合气道、柔术等。西式击剑和亚洲剑术也有不少的跟随者。1990 年后期以来，在可以合法使用枪支的地方，射击受欢迎的程度也越来越高了。大部分黑客喜欢的武术类型都是那些强调精神的自律，放松的意识，以及意念的控制，而不仅仅是单纯的力量、运动精神、以及身体的强健。
- 实实在在学习一种冥想修炼。多年以来黑客中最受欢迎的形式是参禅。（很重要的一点是，参禅和宗教可以说是独立的，你不需要接受一种新宗教，或者放弃现有的宗教信仰，就能做参禅的修炼。其他的形式也许也管用，但注意一定要挑那些靠谱的，不需要你相信不着边际的事物的冥想方式来演练。
- 提高自己对双关语和文字游戏的鉴赏能力。

如果这些事情有很多你已经在做了，那你可能是天生做黑客的材料。至于为什么偏偏是这些事情，原因并不完全清楚，但它们都涉及用到左－右脑能力的综合，这似乎是关键所在（黑客们既需要清晰的逻辑思维，有时又需要偏离逻辑跳出问题的表象）。

最后，还有一些不要去做的事情。

- 不要使用愚蠢的，哗众取宠的ID或昵称。
- 不要卷入 Usenet（或任何其他地方）的骂战。
- 不要自称为“cyberpunk（网络朋克）”，也不要浪费时间和那些人打交道。
- 不要让你的 email 或者帖子中充满错误的拼写和语法。

以上的事情只会为你招来嘲笑。黑客们个个记忆超群——你将需要数年的时间让他们忘记你犯下的错误。

网名的问题值得深思。将身份隐藏在虚假的名字后是骇客、软件破解者、及其他低等生物幼稚愚蠢的行为。黑客不会做这些事；他们对他们所作的感到骄傲，而且乐于人们将作品与他们的真名相联系。因此, 如果你现在还在使用假名，那就放弃它吧。在黑客文化里假名是失败者的标记。


###关于黑客、开源、以及自由软件的历史

1996 年我开始写这篇 HOWTO，那时候的大环境和现在很不一样。这里会给你简单介绍一下相关的历史变迁，这样大致可以澄清一下开源软件、自由软件、以及 Linux 和黑客圈的关系。如果你对这些不感兴趣，你可以直接跳过这一节，继续读下面的 FAQ。

我在这里所描述黑客精神和社会远远早于1990 Linux 出现的时候，我第一次涉足黑客圈是 1976 年，而究其根源则可追溯到20世纪60年代初。但在 Linux 出现之前，大多数黑客使用的操作系统要么是私有的商业版本，要么是自己开发的未得到广泛使用的系统（例如麻省理工学院的 ITS 系统）。虽然那时也有人想要改变这种状况，但他们的努力影响范围相当有限，充其量仅在某个黑客社区有少数忠实用户而已。

现在所谓“开源”历史和黑客社区的历史几乎一样长，但直到 1985 年前，它只是一种没有固定称谓的习惯做法，而不是一套有理论做后盾，有宣言做前锋的自觉运动。这种状态在 1985年结束了，长老级黑客 Richard Stallman（也被称为“RMS”）将其命名为“自由软件 (Free Software)”。这种命名也是一种宣言的方式，不过大多数黑客社区都不接收这种包含明显思想烙印的标签。因此而大多数现有的黑客社区从来没有接受。结果，“自由软件”这一标签被黑客社群中声音较大的少数人（尤其是 BSD Unix 的相关人士）拒绝掉了，而剩下的大部分人（包括我）虽然也有保留意见，可也还是沿用了这一称谓。

尽管很多人存在保留意见，RMS 的“自由软件”的大旗也一直举到了 1990 年代中期。直到 Liunx 崛起时它才受到了重大挑战。Linux 给了的开源开发者一个新的自然归宿，很多项目都已我们现称的开源的方式由 Unix 移植到了 Linux 系统中。Linux 的社区也得到了爆炸性增长，成为了一个比以前黑客文化更为庞大，并且异质化的新的群体。RMS 曾今尝试将这一社群也归并到他的“自由软件运动”大旗下，但终究没有成功，原因可以归于 Linux 社区的样性，以及 Linus Torvalds 本人的质疑。Torvalds 公开拒绝了 RMS 的自由软件思想，但还是沿用了“自由软件”这一术语，这也引来了很多年轻黑客的效仿。

1996年，当我第一次发表这篇 HOWTO 的时候，黑客社团正在围绕着 Linux 和其它几个开源操作系统（尤其是 BSD Unix 的衍生系统）进行着快速的重组。几十年来围绕着闭源系统进行闭源开发的方式还没有开始淡出集体记忆，但在大家看来，这似乎已经是死去的历史了。越来越多的黑客都已经开始注重自己在开源项目（例如 Linux、Apache 等）上的贡献，并将这些贡献当做自己的成就。

然而在那个时候“开源”这一名词还没有出现。这个名词是 1998 年初才开始出现的，而在出现的半年内，大部分的黑客社区就接受了这一名词，只有少数不接受这一概念的人还在坚持使用“自由软件”这一名词。1998 年以后，或者更准确地说是 2003 年以后，所谓的“hacking” 和 “开源（自由）软件开发”的含义已经非常接近了。从今天的眼光来看，这种区分已经没有意义了，看趋势，这个现状将来也不大可能有多大的改变。

不管怎样，这段变更的历史还是值得记住的。


###其它资源

Paul Graham 写了一篇 [http://www.paulgraham.com/gh.html Great Hackers]，还有[http://www.paulgraham.com/college.html Undergraduation]一篇，里边有充满智慧的言论。

还有一篇叫[http://samizdat.mines.edu/howto/HowToBeAProgrammer.html How To Be A Programmer] 的文章，是这篇文章很好的补充。里边的建议不但包括如何提高编程和其它技术，还包含团队合作的窍门。

我还写过一篇 [http://catb.org/~esr/writings/hacker-history/hacker-history.html A Brief History Of Hackerdom] （译注：黑客文化简史）。

我写了一本[http://catb.org/~esr/writings/cathedral-bazaar/index.html The Cathedral and the Bazaar]（译注：大教堂与市集），对于 Linux 及开放源代码文化现象有详细的解释。这种现象在我的另一篇 [http://catb.org/~esr/writings/homesteading/ Homesteading the Noosphere] （译注：开拓智域）中还有更直接的阐述。

Rick Moen 写了一份很好的关于[http://linuxmafia.com/faq/Linux_PR/newlug.html how to run a Linux user group]（译注：如何运营Linux 用户组）的文档。

我和Rick Moen合作完成了另一份关于[http://catb.org/~esr/faqs/smart-questions.html How To Ask Smart Questions]（译注：提问的智慧）的文章，可以让在寻求帮助时得到事半功倍的效果。

如果你想知道 PC、UNIX 及 Internet 基本概念和工作原理，参考[http://en.tldp.org/HOWTO//Unix-and-Internet-Fundamentals-HOWTO/ The Unix and Internet Fundamentals HOWTO]。

当你发布软件或者补丁的时候，请遵照[http://en.tldp.org/HOWTO/Software-Release-Practice-HOWTO/index.html Software Release Practice HOWTO] 去做。

如果你对禅诗感兴趣，也许你还喜欢看这篇[http://catb.org/~esr//writings/unix-koans Rootless Root: The Unix Koans of Master Foo]


###FAQ（常见问题解答）


####怎样才能知道自己已经是一名够格的黑客

你可以问自己下面三个问题：

- 你能流利地读写代码吗？
- 你认同黑客社群的目的和价值吗？
- 黑客社群里有没有资深成员称呼你为黑客呢？

如果你对这三个问题的答案都是“是”的话，你已经是一名黑客了。如果你只满足其中两项，那就说明你还不够格。

第一个问题是关于技能的。如果你已经符合本文前面提到的最低需求的话，你也算过关，不过如果你发布过为数不少的开源代码并被社群接受，那你就算满分过关了。

第二个问题是关于态度的。如果黑客精神的五项基本原则对你来说能有共鸣，而且已经是你处事的方式，你就算过关一半了。这算靠里的一半，靠外的一半和你在黑客社区长期项目上的投入和关联程度有关。

这里列出了一些项目的不完全列表供你参考：Linux 的改进和用户群扩大对你来说是否重要？你对于自由软件精神是否充满激情？你对于垄断是否有敌意？你是否相信计算机这种工具会让增加世界财富，让这个世界更富有人道主义？

不过值得注意的一点是，黑客社群有一些特有的政治倾向，其中两条，一条是保卫言论自由权，一种是抵御所谓“知识产权”对于开源社区的侵害。实践这两条的是一些民间组织，例如电子前沿基金会（Electronic Frontier Foundation）就是其中之一。不过虽然如此，黑客们对于有任何明确政治目的的团体都是心怀戒备的，因为我们已经从各种经验教训中学到一点：这些活动只会分裂黑客社团，并让黑客们分心。如果有人以黑客精神为名组织一场首都大游行，那他就完全没有弄明白这点。真正的应对方式也许应该是“闭上嘴巴，给他们看代码”。

第三个问题有点循环递归的味道。在“什么是黑客”一节我已经讲过，作为一名黑客的意义在于参与某个黑客社群，也就是社交网络的一个亚文化团体，作为内部的贡献成员以及外部的宣传者积极活动。和很久以前相比，黑客群体现在的团结意识和自我意识已经增强了很多。过去三十年来，随着互联网的发展，社交网络逐渐开始发挥举足轻重的作用，而黑客的亚文化团体也更加容易发展和维护了。这种变革的明显一个有代表性的现象是：有的黑客社群现在都有自己专门的文化衫了。

研究社交网络的社会学家把黑客文化归为“看不见的大学”，而且注意到这些网络社交圈还有所谓的“看门人”——其中的一些核心成员，他们有一定的权威，可以准新成员的进入。所谓的“看不见的大学”本来就是一个松散的非正式组织，所以这些“看门人”也只是这门称呼而已。但不是每个黑客都是“看门人”，这是每个黑客都深刻明白的一点。“看门人”需要有一定的资历和成就，究竟要到什么程度很难讲，但一旦有这样的人出现，每一个黑客都能辨识出来。


####你能教我做黑客吗

自从第一次发布这份文档，我每周都会收到一些请求，（频繁的话一天几封）要我“教会他们做黑客”。遗憾的是，我 没有时间和精力来做这个；我自己的黑客项目，及我作为一个开放源代码倡导者 的四处奔波已经占用了我110%的时间。

即便我想教你，黑客也依然基本上是一项自行修炼的的态度和技术。 当真正的黑客想帮助你的时候，如果你乞求他们一汤匙一汤匙“喂”你的话，你会发现他们不会尊重你。

先去学一些东西。显示你在尝试，你能靠自己去学习。然后再去向你遇到的黑客请教特殊的问题。

如果你发E-mail给一位黑客寻求他的帮助，这是两件首要记住的事情。 第一，写出来的文字显得懒且粗心的人通常非常懒于思考且非常马大哈，不能成为好黑客——因此注意拼写正确，使用正确的语法及发音，否则你可能会无人理睬。 第二，不要试图要求回复到一个ISP帐号，而那个帐号与你 的发信地址不同。这样做的人一般是使用盗用帐号，我们对于回报或者帮助窃贼不感兴趣。


####那么，我要如何开始

对你而言最佳的入门方式也许是去参加 LUG（Linux用户组）的聚会。 你可以找到在 LDP 的综合 Linux 信息页面上找到类似的组织；也许有一个在你家附近的，而且非常有可能与一所大学或学校挂钩。如果你提出要求，LUG 成员兴许会给你一套 Linux，当然此后会帮你安装并带你入门。


####我得什么时候开始学？现在会不会太迟了？

你有动力学习的时候就是好时候。大多数人看来都是在15－20岁之间开始感兴趣的，但据我所知，在此年龄段之外的例外也是有的。


####要学多久才能学会黑客技能？

这取决于你的聪明程度和努力程度。对于大多数人，只要足够专注，就能在 18 个月到 2 年之间学会一套令人尊敬的技能。但是，不要以为这样就够了；如果你是一个真正的黑客，你要用你的余生来学习和完善你的技术。


####Visual Basic 是好的入门语言吗？

既然你问了这个问题，那你肯定是想在 Microsoft Windows 操作系统下学习黑客技能。这本身就不是一个好主意。我前面讲过在 Windows 下 hack 就跟穿着骑士铠甲跳舞一样，我不是在开玩笑。别走这条路，Windows 是一个很低劣的 hack 环境，而且一直如此。

Visual Basic 有一个特征性问题，就是它不可以被移植到其他平台。虽然也有些 Visual Basic 开源实现的雏形，但实现的只是 ECMA 标准的一个很小的子集。在 Windows 下大部分类库的知识产权都是 Microsoft 独家所有，如果你不是及其小心的话，你的代码将只能在 Microsoft 支持的平台上使用。如果你不打算从 Unix 起步，那你也有更好的语言可选，而且类库质量还更高，例如 Python 就是其中之一

和其他的 Basic 类语言一样，Visual Basic 这门编程语言的设计也很糟糕，它会教你一些坏的变成习惯。你就别问我细节了，这可是罄竹难书。还是去学一门设计优良的语言吧。

其中一个坏习惯是让你依赖于单一厂商的函数库、控件及开发工具。一般而言，任何不能够支持至少 Linux 或者某一种 BSD，或其不能支持至少三种以上操作系统的语言，都是一种不适合应付黑客工作的语言。


####你能帮我“黑”掉一个站点吗？或者教我怎么黑它？

No。任何读完这份 FAQ 后还问这个问题的人，都是无可救药的蠢材，即使有时间指教我也不会理睬。任何发给我的此类电子邮件都会被忽略或被痛骂一顿。


####我怎么样才能得到别人帐号的密码？

这是骇客行为。滚得远远的，白痴。


####我如何入侵/查看/监视别人的 Email？

这是骇客行为。在我面前消失，智障。


####我如何才能在IRC聊天室里偷到频道 op 的特权？

这是骇客行为。滚开，笨蛋。


####我被黑了。你能帮我避免以后再被攻击吗？

不行。目前为止，每次问我这个问题的，都是一些运行 Microsoft Windows 的菜鸟。不可能有效的保护 Windows 系统免受骇客攻击；太多代码和架构的缺陷使保护 Windows 的努力有如隔靴搔痒。唯一可靠的预防来自转移到 Linux 或其他设计得至少足够安全的系统。


####我的 Windows 软件出现问题了。你能帮我吗？

当然。打开 DOS 命令行输入“format c:”。你遇到的任何问题将会在几分钟之内消失。


####我在哪里能找到可以与之交流的真正的黑客？

最佳办法是在你附近找一个Unix或Linux的用户组，参加他们的聚会。（你可以在 ibiblio 的 LDP 站点找到一些用户组的链接。）

（我过去曾说过不能在IRC上找到真正的黑客，但我发觉现在情况有所改变。显然一些真正的黑客的社区像 GIMP 及 Perl，也有IRC频道了。）
你能推荐一些有关黑客的好书吗？

我维护着一份[http://en.tldp.org/HOWTO/Reading-List-HOWTO/index.html Linux Reading List HOWTO]，也许你会觉得有用。[http://catb.org/~esr/faqs/loginataka.html The Loginataka] 也大致值得一读。

关于Python的介绍，请访问在Python站点上的[http://sebug.net/paper/python/ 入门教程]。


####成为一名黑客我需要擅长数学吗？

不用。黑客道很少使用常规的数学或算术，不过你绝对需要能逻辑性地思考和进行精密的推理。尤其是你不会用到微积分或电路分析（我们把这些留给电子工程师们 :-)）。有限数学中的一些可提（包括布尔代数，集合论，组合数学，图论）的背景知识会对你有所帮助。

更重要的一点：你要有逻辑思维能力，能够以数学家的方式追溯因果。虽然大部分的数学知识对你可能没什么用处，但数学思维的能力对你来说是极其重要的。如果你缺乏这方面的智慧，要做一名黑客恐怕是无望了。如果你缺乏这方面的训练，还是尽早开始吧。


####我该从那种语言学起

如果你还没学过XHTML（HTML最新的表现形式）的话，就从它开始吧。市面上有一大堆的封面精美，宣传得天花乱坠的HTML 书籍，不幸的是质量优秀的几近于无。我最喜欢的是[http://www.oreilly.com/catalog/html5/ HTML: The Definitive Guide]。

但HTML 不是一种完整的编程语言。当你准备开始编程时，我推荐从[http://sebug.net/paper/python/ Python]起步。 你会听到一大群人推荐 Perl，但是 Perl 要难学得多，而且（以我之见）设计得不是很好。

C 确实重要，但它也比 Python 或 Perl 难多了。不要尝试先学 C。

Windows用户注意：不要满足于 Visual Basic。它会教给你坏习惯，而且它不可以跨平台移植，只能在Windows下运行。因此还是敬而远之为好。


####我需要什么样的机器配置

过去个人电脑能力相当不足并且内存很小，这给黑客的学习过程设置了人为的障碍。不过 1990 中期以后就不是这样了；任何一台 Intel 486DX50 以上配置的机器都有足够的能力进行开发工作、运行 X 系统、以及进行 Internet 通讯。而且你买到的市面上最小的硬盘都大得足够你使用了。

选择用来学习的机器时重要的一点是注意配件是否是Linux兼容的（或BSD兼容，如果你选择 BSD 的话）。和刚才提到的一样，大多数现在的机器都是符合的；唯一值得注意的区域在于 modem 和打印机；有些具备为Windows设计的配件的机器不会在Linux下工作。


####我想贡献社区。你可以帮我选一个问题让我下手吗？

不行，因为我不知道你的兴趣和擅长领域在哪里。如果你没有内在动力，你就很难坚持下去，所以说，别人只给你的路是行不通的。

试试这么做吧。在 Freshmeat 网站观察几天，看看里边的项目更新，如果你看到一个看上去很酷而且你也很感兴趣的项目，就加入吧。


####我得因此憎恨和反对 Microsoft 吗

不，你不必如此。不是因为Microsoft不令人讨厌，而是因为黑客文化早在 Microsoft 出现之前就存在了，且将在 Microsoft 成为历史后依然存在。 你耗费在憎恨 Microsoft 的任何力气不如花在爱你的技术上。写好的代码——那会相当有效地打击 Microsoft 又不会让你得到恶报应。


####开放源代码软件不会使程序员丢饭碗吗

目前看起来不太可能，开放源代码软件产业似乎创造了更多的就业机会而不是减少就业机会。如果写一个程序比起不写来是纯经济收益的话，那么在写完后，程序员应该得到报酬不管程序是否是开放源代码。并且，无论写出多么“免费自由”的软件，都存在更多对新的，定制的软件的需求。我有这方面更多的论述，放在放源代码网站资料中。


####我要如何开始？哪里有免费的Unix

在本份文档的某个地方我已经提到过何处可以得到最常用的免费 Unix。要做一名黑客，你需要自己找到激励和动力，还要有自学的能力。现在就开始努力吧……


>
> Eric Steven Raymond
> Thyrsus Enterprises
> Copyright © 2001 Eric S. Raymond <esr@thyrsus.com>
> Wang Dingwei <wangdingwei82@gmail.com> 基于 Barret 的翻译更正而成。转载请注明出处。
>