# Challenge 2 : Redirecting More Output

Developed an understanding of output redirection using the > character

## My solve

**Flag:** pwn.college{MohKNAA3dhuG-F2kIBfzZmi-Mrf.QX1YTN0wiN3gjNzEzW}

What I Learnt: How to use > to redirect output

- As the challenge asked I used > to redirect the output of /challenge/run into myflag to obtain the flag

```
hacker@piping~redirecting-more-output:~$ /challenge/run > myflag
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : myflag
[INFO] - the challenge will output a reward file if all the tests pass : /flag

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /flag file.

[TEST] You should have redirected my stdout to a file called myflag. Checking...

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~redirecting-more-output:~$ myflag
bash: myflag: command not found
hacker@piping~redirecting-more-output:~$ ls
COLLEGE  myflag  not-the-flag  r
hacker@piping~redirecting-more-output:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{MohKNAA3dhuG-F2kIBfzZmi-Mrf.QX1YTN0wiN3gjNzEzW}
```

Incorrect Tangents :
Forgot to use the cat command to read out the flag

References :
None
