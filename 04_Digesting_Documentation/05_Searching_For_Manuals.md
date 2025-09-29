# Challenge 5 : Searching For Manuals

Developed an understanding of the man command and how to navigate inside the manual

## My solve

**Flag:** pwn.college{QbfZp1hz-pd-Ojy7b9PEssUBPwI.QX2EDO0wiN3gjNzEzW}

What I Learnt: Understood how to navigate and search inside the manual by using the arrow keys and /.

- Used man man to find out the argument used to find out manual names for files and got the manual name for the challenge file and then used correct argunment with /challenge/challenge to get the flag

```
hacker@man~searching-for-manuals:~$ man man
hacker@man~searching-for-manuals:~$ man -k challenge
bfphzpdjyb (1)       - print the flag!
hacker@man~searching-for-manuals:~$ man bfphzpdjyb
hacker@man~searching-for-manuals:~$ /challenge/challenge --bfphzp 179
Correct usage! Your flag: pwn.college{QbfZp1hz-pd-Ojy7b9PEssUBPwI.QX2EDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
