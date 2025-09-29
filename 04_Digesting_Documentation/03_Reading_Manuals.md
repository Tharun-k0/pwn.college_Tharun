# Challenge 3 : Reading Manuals

Developed an understanding of the man command

## My solve

**Flag:** pwn.college{Q6YvV2MSa8pNReJUi4dOktDFjJV.QX0EDO0wiN3gjNzEzW}

What I Learnt: Understood how the man command works.

- Used man to get the manual for the challenge and then used the correct argunment with /challenge/challenge to get the flag

```
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge vapeid 628
Incorrect usage! Please read the challenge man page!
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge  --vapeid 628
Correct usage! Your flag: pwn.college{Q6YvV2MSa8pNReJUi4dOktDFjJV.QX0EDO0wiN3gjNzEzW}
```

Incorrect Tangents :
Forgot to put -- before the --vapeid NUM argument resulting in an error

References :
None
