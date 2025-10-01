# Challenge 12 : Writing To Multiple Programs

Developed an understanding of duplicating output of a program as input into multiple programs using tee

## My solve

**Flag:** pwn.college{8XFAQCjuUkOmK1uOTgcsYagCYRz.QXwgDN1wiN3gjNzEzW}

What I Learnt: How to use tee to write output of a program into multiple programs as input to get desired output

- Used tee and | to write the output of /challenge/hack into the stdin of /challenge/the and /challenge/planet to get the flag

```
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >(/challenge/the) | tee >(/challenge/planet)
This secret data must directly and simultaneously make it to /challenge/the and
/challenge/planet. Don't try to copy-paste it; it changes too fast.
17278158711411731229
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{8XFAQCjuUkOmK1uOTgcsYagCYRz.QXwgDN1wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
