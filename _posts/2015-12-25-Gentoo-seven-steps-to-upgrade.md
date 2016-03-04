There is no a full HOWTO introducing whole system upgrading. I hope this simple document can help someone else.

src: https://forums.gentoo.org/viewtopic-t-807345.html

1. sync portage tree(eix-sync is recommended)

```
# eix-sync  
```

or

```
# emerge --sync
```

2. upgrade whole system

```
# emerge -avuDN --with-bdeps y --keep-going world   
```

3. make configuration file(s) up to date

```
# etc-update    
```

or

```
# dispatch-conf 
```

4. fix static library

```
# lafilefixer --justfixit | grep -v skipping
```

5. uninstall useless packages

```
# emerge -av --depclean 
```

6. Reverse dynamic library Dependency

```
# revdep-rebuild
```

7. clean source code of the old packages

```
# eclean -d distfiles
```
