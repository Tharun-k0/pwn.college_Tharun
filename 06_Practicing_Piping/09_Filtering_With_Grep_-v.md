# Challenge 9 : Filtering With grep -v

Developed an understanding of using -v (invert match) with grep

## My solve

**Flag:** pwn.college{cldJ_c9Pf-MFxfB1WTSrXWykq7a.0FOxEzNxwiN3gjNzEzW}

What I Learnt: How to use -v with grep to invert match the string

- I used grep -v to filter out all the fake flags as all of them had the string "DECOY" as mentioned in the challenge to get the required flag

```
hacker@piping~filtering-with-grep-v:~$ /challenge/run | grep -v DECOY
pwn.college{cldJ_c9Pf-MFxfB1WTSrXWykq7a.0FOxEzNxwiN3gjNzEzW}
hacker@piping~filtering-with-grep-v:~$
```

Incorrect Tangents :
None

References :
None
