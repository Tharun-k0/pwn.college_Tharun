# Challenge 7 : Helpful Programs

Developed an understanding of the help builtin

## My solve

**Flag:** pwn.college{wPLZIMqWkrsu7IccWrF1QGHdHkp.QX0ETO0wiN3gjNzEzW}

What I Learnt: Understood how to use the help builtin to find details about programs

- Used help with challenge as a builtin to figure out correct arguments to get the flag

```
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "wPLZIMqW".
hacker@man~help-for-builtins:~$ challenge --secret wPLZIMqW
Correct! Here is your flag!
pwn.college{wPLZIMqWkrsu7IccWrF1QGHdHkp.QX0ETO0wiN3gjNzEzW}
```

Incorrect Tangents :
Accidentally used the wrong syntax for the command to run the program

References :
None
