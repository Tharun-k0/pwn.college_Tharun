# Challenge 1 : Matching With \*

Developed an understanding of first glob \*

## My solve

**Flag:** pwn.college{4kU1A4EzB9n-lq5kIyoOQDZxL6G.QXxIDO0wiN3gjNzEzW}

What I Learnt: Understood how to use the \* glob

- Used \* to cd to /challenge directory in under 4 characters and then ran /challenge/run to get the flag

```
This challenge resets your working directory to /home/hacker unless you change
directory properly...
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{4kU1A4EzB9n-lq5kIyoOQDZxL6G.QXxIDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
