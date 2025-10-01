# Challenge 2 : Matching With ?

Developed an understanding of second glob ?

## My solve

**Flag:** pwn.college{oIibJjj0h85W9N2YoXfqyurRYsz.QXyIDO0wiN3gjNzEzW}

What I Learnt: Understood how to use the ? glob

- Used ? to cd to /challenge directory using ? instead of c and l in the name of the directory and then ran /challenge/run to get the flag

```
This challenge resets your working directory to /home/hacker unless you change
directory properly...
This challenge resets your working directory to /home/hacker unless you change
directory properly...
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{oIibJjj0h85W9N2YoXfqyurRYsz.QXyIDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
