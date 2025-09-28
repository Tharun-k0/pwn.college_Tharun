# Challenge 7 : Touching Files

Developed an understanding of the touch command

## My solve

**Flag:** pwn.college{EXHOU7P7HqRAnlQIjW4yNsudiMw.QXwMDO0wiN3gjNzEzW}

What I Learnt: Understood the working of the touch command

- Used the touch command to create two new files in /tmp and obtain the flag by running /challenge/run

```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ ls
bin  hsperfdata_root  pwn  tmp.4mK6TfTSUV
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ cd
hacker@commands~touching-files:~$ /challenge/run
Success! Here is your flag:
pwn.college{EXHOU7P7HqRAnlQIjW4yNsudiMw.QXwMDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
