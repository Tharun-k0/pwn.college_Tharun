# Challenge 6 : Grepping Stored Results

Developed an understanding of using grep together with redirecting

## My solve

**Flag:** pwn.college{gSsoEnjjqGbi7awOzVym2fI-4Z7.QX4EDO0wiN3gjNzEzW}

What I Learnt: How to use > to redirect out and then use grep to filter out required data

- As the challenge asked I used > to redirect output of /challenge/run into /tmp/data.txt and then grep using the string as pwn.college as all the flags start with it and obtain the flag

```
hacker@piping~grepping-stored-results:~$ /challenge/run > /tmp/data.txt
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge will check that output is redirected to a specific file path : /tmp/data.txt
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stdout to a file called /tmp/data.txt. Checking...

[HINT] File descriptors are inherited from the parent, unless the FD_CLOEXEC is set by the parent on the file descriptor.
[HINT] For security reasons, some programs, such as python, do this by default in certain cases. Be careful if you are
[HINT] creating and trying to pass in FDs in python.

[PASS] The file at the other end of my stdout looks okay!
[PASS] Success! You have satisfied all execution requirements.
hacker@piping~grepping-stored-results:~$ grep pwn.college /tmp/data.txt
pwn.college{gSsoEnjjqGbi7awOzVym2fI-4Z7.QX4EDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
