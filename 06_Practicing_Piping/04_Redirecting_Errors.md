# Challenge 4 : Redirecting Errors

Developed an understanding of error redirection using FD 2 with >

## My solve

**Flag:** pwn.college{0xYTSnThWrO1NEfZ09E07IbyP3r.QX3YTN0wiN3gjNzEzW}

What I Learnt: How to use 2> to redirect errors

- As the challenge asked I used > and 2> to redirect the output and instructions from /challenge/run to myflag and instructions respectively

```
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ ls
COLLEGE  instructions  myflag  not-the-flag  r  the-flag
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{0xYTSnThWrO1NEfZ09E07IbyP3r.QX3YTN0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
