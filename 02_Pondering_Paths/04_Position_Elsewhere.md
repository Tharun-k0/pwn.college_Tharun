# Challenge 4 : Position Elsewhere

Had to navigate to a directory using the cd command and then invoke a program in this challenge.
(Same as previous challenge)

## My solve

**Flag:** pwn.college{QLc81HNsxut8ImhFEaFjPeuVo4r.QX3QTN0wiN3gjNzEzW}

What I Learnt:The cd command,directories, absolute path and how to navigate directories using the cd command and invoking programs inside it using absolute path.

- Navigated to given directory using the cd command "cd /usr/share/build-essential" and then executed the
  "/challenge/run" program

```
hacker@paths~position-elsewhere:~$ cd /usr/share/build-essential
hacker@paths~position-elsewhere:/usr/share/build-essential$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{QLc81HNsxut8ImhFEaFjPeuVo4r.QX3QTN0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
