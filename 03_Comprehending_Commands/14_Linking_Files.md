# Challenge 14 : Linking Files

Developed an understanding of the ln -s command and the find command

## My solve

**Flag:** pwn.college{Urtfl3-h1TFNo7cE1mpK6rtOcFl.QX5ETN1wiN3gjNzEzW}

What I Learnt: Understood the working of the ln -s and the find command

- Used the ln -s command to link the flag to the not-the-flag file and then run /challenge/catflag which reads out the not-the-flag file to obtain the flag

```
hacker@commands~linking-files:~$ ln -s /flag ~/not-the-flag
hacker@commands~linking-files:~$ ls
not-the-flag  r
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{Urtfl3-h1TFNo7cE1mpK6rtOcFl.QX5ETN1wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
