# Challenge 11 : An Epic File System Quest

Using the knowledge gained about new commands from the previous challenges in the module, I had to use ls, ls -a, cd, and cat commands multiple times to navigate towards the flag

## My solve

**Flag:** pwn.college{k0GMkEtZ5cNk0A9k4eI2tvMb5vF.QX5IDO0wiN3gjNzEzW}

What I Learnt: Application of the commands learnt

- Used the cd, ls, cat commands multiple times and used the absolute path with the ls and cat commands when cd'ing was not allowed and also used the ls -a command to show hidden files in the challenge.

```
hacker@commands~an-epic-filesystem-quest:~$ cd /
hacker@commands~an-epic-filesystem-quest:/$ ls
HINT  bin  boot  challenge  dev  etc  flag  home  lib  lib32  lib64  libx32  media  mnt  nix  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
hacker@commands~an-epic-filesystem-quest:/$ cat HINT
Congratulations, you found the clue!
The next clue is in: /opt/pwndbg/.venv/lib/python3.8/site-packages/cffi
hacker@commands~an-epic-filesystem-quest:/$ cd /opt/pwndbg/.venv/lib/python3.8/site-packages/cffi
hacker@commands~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/cffi$ ls
TIP          _cffi_errors.h   _imp_emulation.py       backend_ctypes.py  cparser.py      lock.py         pkgconfig.py       vengine_cpy.py
__init__.py  _cffi_include.h  _shimmed_dist_utils.py  cffi_opcode.py     error.py        model.py        recompiler.py      vengine_gen.py
__pycache__  _embedding.h     api.py                  commontypes.py     ffiplatform.py  parse_c_type.h  setuptools_ext.py  verifier.py
hacker@commands~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/cffi$ cat TIP
Tubular find!
The next clue is in: /opt/libslub/.git/objects/5b

The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'.
hacker@commands~an-epic-filesystem-quest:/opt/pwndbg/.venv/lib/python3.8/site-packages/cffi$ cd /opt/libslub/.git/objects/5b
hacker@commands~an-epic-filesystem-quest:/opt/libslub/.git/objects/5b$ ls
TEASER  c3db623b468a400f97401ba2ca56ca752db003
hacker@commands~an-epic-filesystem-quest:/opt/libslub/.git/objects/5b$ cat TEASER
Tubular find!
The next clue is in: /usr/lib/firefox-addons/extensions

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/opt/libslub/.git/objects/5b$ ls /usr/lib/firefox-addons/extensions
BLUEPRINT-TRAPPED
hacker@commands~an-epic-filesystem-quest:/opt/libslub/.git/objects/5b$ cat /usr/lib/firefox-addons/extensions/BLUEPRINT-TRAPPED
Lucky listing!
The next clue is in: /usr/lib/jvm/java-11-openjdk-amd64/legal/jdk.jshell
hacker@commands~an-epic-filesystem-quest:/opt/libslub/.git/objects/5b$ cd /usr/lib/jvm/java-11-openjdk-amd64/legal/jdk.jshell
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-11-openjdk-amd64/legal/jdk.jshell$ ls
ASSEMBLY_EXCEPTION  MESSAGE
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-11-openjdk-amd64/legal/jdk.jshell$ cat MESSAGE
Yahaha, you found me!
The next clue is in: /opt/busybox/busybox-1.33.2/mailutils

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-11-openjdk-amd64/legal/jdk.jshell$ ls /opt/busybox/busybox-1.33.2/mailutils
ALERT-TRAPPED  Config.src  Kbuild.src  lib.a   mail.h  makemime.c  popmaildir.c  reformime.c  sendmail.c
Config.in      Kbuild      built-in.o  mail.c  mail.o  makemime.o  popmaildir.o  reformime.o  sendmail.o
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-11-openjdk-amd64/legal/jdk.jshell$ cat /opt/busybox/busybox-1.33.2/mailutils/ALERT-TRAPPED
Lucky listing!
The next clue is in: /usr/local/lib/python3.8/dist-packages/idna-3.10.dist-info

The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'.
hacker@commands~an-epic-filesystem-quest:/usr/lib/jvm/java-11-openjdk-amd64/legal/jdk.jshell$ cd /usr/local/lib/python3.8/dist-packages/idna-3.10.dist-info
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/idna-3.10.dist-info$ ls -a
.  ..  .WHISPER  INSTALLER  LICENSE.md  METADATA  RECORD  WHEEL
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/idna-3.10.dist-info$ cat .WHISPER
Tubular find!
The next clue is in: /opt/linux/linux-5.4/drivers/crypto/axis

Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/idna-3.10.dist-info$ ls /opt/linux/linux-5.4/drivers/crypto/axis
LEAD-TRAPPED  Makefile  artpec6_crypto.c
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/idna-3.10.dist-info$ cat /opt/linux/linux-5.4/drivers/crypto/axis/LEAD-TRAPPED
Yahaha, you found me!
The next clue is in: /opt/linux/linux-5.4/drivers/staging/android/uapi
hacker@commands~an-epic-filesystem-quest:/usr/local/lib/python3.8/dist-packages/idna-3.10.dist-info$ cd /opt/linux/linux-5.4/drivers/staging/android/uapi
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/staging/android/uapi$ ls
INSIGHT  ashmem.h  ion.h  vsoc_shm.h
hacker@commands~an-epic-filesystem-quest:/opt/linux/linux-5.4/drivers/staging/android/uapi$ cat INSIGHT
CONGRATULATIONS! Your perserverence has paid off, and you have found the flag!
It is: pwn.college{k0GMkEtZ5cNk0A9k4eI2tvMb5vF.QX5IDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
