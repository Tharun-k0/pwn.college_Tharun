# Challenge 12 : Making Directories

Developed an understanding of the mkdir command

## My solve

**Flag:** pwn.college{ElM_Lf_BbZnBVZx4IbjYoaj9uSD.QXxMDO0wiN3gjNzEzW}

What I Learnt: Understood the working of the mkdir command

- Used the mkdir command to create a directory in the /tmp directory and then create a file using touch in the new directory and ran /challenge/run to get the flagS

```
hacker@commands~making-directories:~$ cd /tmp
hacker@commands~making-directories:/tmp$ mkdir pwn
hacker@commands~making-directories:/tmp$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ ls
college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{ElM_Lf_BbZnBVZx4IbjYoaj9uSD.QXxMDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
