# Challenge 5 : Comparing Files

Developed an understanding of the diff command

## My solve

**Flag:** pwn.college{ELsPtv0hrdrjUGwZIa9yJQ6po3k.01MwMDOxwiN3gjNzEzW}

What I Learnt: Understood the working of the diff command

- Searched for the flag by going to required dir and then comparing the decoys only file with the decoys and real file by using the diff command to get the real flag

```
hacker@commands~comparing-files:~$ cd /challenge
hacker@commands~comparing-files:/challenge$ diff decoys_only.txt decoys_and_real.txt
51a52
> pwn.college{ELsPtv0hrdrjUGwZIa9yJQ6po3k.01MwMDOxwiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
