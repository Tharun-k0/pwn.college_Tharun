# Challenge 5 : Redirecting Input

Developed an understanding of input redirection using <

## My solve

**Flag:** pwn.college{w3VBsKtey\_\_ZJ_0qkbgkFfvYtMu.QXwcTN0wiN3gjNzEzW}

What I Learnt: How to use < to redirect input

- I used > to redirect COLLEGE into PWN and then use < to redirect PWN as input into /challenge/run to get the flag

```
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{w3VBsKtey__ZJ_0qkbgkFfvYtMu.QXwcTN0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
