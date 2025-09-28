# Challenge 10 : Hidden Files

Developed an understanding of invoking ls with the -a flag to view hidden files in a directory

## My solve

**Flag:** pwn.college{QC8GDv0WDFjH6EBaJWWuYPEmLEq.QXwUDO0wiN3gjNzEzW}

What I Learnt: Understood the working of the -a flag with the ls command

- Used the ls command with the -a flag to view the flag file and then used cat to read the flag

```
hacker@commands~hidden-files:~$ cd /
hacker@commands~hidden-files:/$ ls
bin  boot  challenge  dev  etc  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~hidden-files:/$ ls -a
.   .dockerenv             bin   challenge  etc   lib    lib64   media  nix  proc  run   srv  tmp  var
..  .flag-121571590624613  boot  dev        home  lib32  libx32  mnt    opt  root  sbin  sys  usr
hacker@commands~hidden-files:/$ .flag-121571590624613
bash: .flag-121571590624613: command not found
hacker@commands~hidden-files:/$ cat .flag-121571590624613
pwn.college{QC8GDv0WDFjH6EBaJWWuYPEmLEq.QXwUDO0wiN3gjNzEzW}
```

Incorrect Tangents :
Tried to

References :
None
