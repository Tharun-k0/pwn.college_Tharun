# Challenge 4 : Exporting Variables

Developed an understanding of how to export variables

## My solve

**Flag:** pwn.college{U3400xfsghhwzxyRCLEKWKeBKZP.QXyYTN0wiN3gjNzEzW}

What I Learnt: How to use export values of variables

- As told in the challenge I just assigned the value COLLEGE to PWN and vice versa but exported PWN and then ran /challenge/run in a new shell

```
hacker@variables~exporting-variables:~$ COLLEGE=PWN
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ export PWN=COLLEGE
You've set the PWN variable to the proper value!
You've set the COLLEGE variable to the proper value!
hacker@variables~exporting-variables:~$ sh
sh-5.2$ /challenge/run
CORRECT!
You have exported PWN=COLLEGE and set, but not exported, COLLEGE=PWN. Great
job! Here is your flag:
pwn.college{U3400xfsghhwzxyRCLEKWKeBKZP.QXyYTN0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
