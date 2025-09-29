# Challenge 4 : Searching Manuals

Developed an understanding of the man command and how to navigate inside the manual

## My solve

**Flag:** pwn.college{ITA1hrZzl6oh60XpSduKgR1FbOp.QX1EDO0wiN3gjNzEzW}

What I Learnt: Understood how to navigate and search inside the manual by using the arrow keys and /.

- Used man to find out the correct argument for the challenge program and obtained the flag.

```
hacker@man~searching-manuals:~$ man challenge

gzip: stdout: Broken pipe
hacker@man~searching-manuals:~$ /challenge/challenge -g
Initializing...
Correct usage! Your flag: pwn.college{ITA1hrZzl6oh60XpSduKgR1FbOp.QX1EDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None

(I accidentally closed the tab after completing this so my challenge was already completed and i had to do it a second time for a new flag to get the bash and the flag and gzip: stdout: Broken pipe came up while trying to do that.)
