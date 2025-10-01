# Challenge 13 : Split Piping stderr And stdout

Developed an understanding of duplicating output of a program as input into multiple programs using tee

## My solve

**Flag:** pwn.college{sL5cQ5VEhQQXBzKS1oDKnZs-p0e.QXxQDM2wiN3gjNzEzW}

What I Learnt: How to use piping to get stdout and stderr on two different programs

- I used 2> to first of all get the std err in /challenge/the and then piped the output onto /challenge/planet

```
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack 2> >(/challenge/the) | /challenge/planet
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{sL5cQ5VEhQQXBzKS1oDKnZs-p0e.QXxQDM2wiN3gjNzEzW}
```

Incorrect Tangents :
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack |/challenge/planet | 2> >(/challenge/the)

References :
None
