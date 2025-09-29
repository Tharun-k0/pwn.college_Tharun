# Challenge 6 : Helpful Programs

Developed an understanding of the --help argument

## My solve

**Flag:** pwn.college{UdVN8x87Y2sKtWm16_XB1DuhgUS.QX3IDO0wiN3gjNzEzW}

What I Learnt: Understood how to use the --help argument to find details about programs

- Used --help with /challenge/challenge to figure out correct arguments to use with the program to get the flag

```
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 887
hacker@man~helpful-programs:~$ /challenge/challenge -g GIVE_THE_FLAG 887
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]
a challenge to make you ask for help: error: argument -g/--give-the-flag: invalid int value: 'GIVE_THE_FLAG'
hacker@man~helpful-programs:~$ /challenge/challenge -g 887
Correct usage! Your flag: pwn.college{UdVN8x87Y2sKtWm16_XB1DuhgUS.QX3IDO0wiN3gjNzEzW}
```

Incorrect Tangents :
Incorrect syntax for the command

References :
None
