# Challenge 10 : Duplicating Piped Data With tee

Developed an understanding of tee to duplicate piped data into multiple files along with stdout

## My solve

**Flag:** pwn.college{4jxHSSWXdrQ2ycrihlo5IO5D-jv.QXxITO0wiN3gjNzEzW}

What I Learnt: How to use tee to get copies of stdout

- Used tee to get a copy of the piped data and then used cat to find out the argument needed to access the flag and then used it to obtain the flag

```
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee requirements | /challenge/college
Processing...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat requirements
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "4jxHSSWX"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 4jxHSSWX | /challenge/college
Processing...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{4jxHSSWXdrQ2ycrihlo5IO5D-jv.QXxITO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
