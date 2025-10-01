# Challenge 6 : Matching Globs

Developed an understanding of using different globs in a single argument

## My solve

**Flag:** pwn.college{UtXRyBp-e7eEsXTr68cJpDz0wAJ.QX1IDO0wiN3gjNzEzW}

What I Learnt: How to use multiple different globs in a single arguument

- As the challenge asked I cded to /challenge/files directory and used both bracket-glob and _ in the argument as I observed that no other file was starting with the same letters as the ones we needed so i used [cep]_ to include all the required files and get the flag.

```
hacker@globbing~mixing-globs:~$ cd /challenge/files
hacker@globbing~mixing-globs:/challenge/files$ ls
amazing    challenging  educational  great  incredible  kind      magical  optimistic  queenly  splendid   uplifting   wonderful  youthful
beautiful  delightful   fantastic    happy  jovial      laughing  nice     pwning      radiant  thrilling  victorious  xenial     zesty
hacker@globbing~mixing-globs:/challenge/files$ /challenge/run [cep]*
You got it! Here is your flag!
pwn.college{UtXRyBp-e7eEsXTr68cJpDz0wAJ.QX1IDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
