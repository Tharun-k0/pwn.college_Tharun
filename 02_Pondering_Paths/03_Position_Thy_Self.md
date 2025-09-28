# Challenge 3: Position Thy Self

Had to navigate to a directory using the cd command and then invoke a program in this challenge.

## My solve

**Flag:** pwn.college{EvbWmXqBtOn77r2Hvsd1fjuwZIc.QX2QTN0wiN3gjNzEzW}

What I Learnt :The cd command,directories, absolute path and how to navigate directories using the cd command and invoking programs inside it using absolute path.

- Navigated to given directory using the cd command "cd /usr/share/build-essential" and then executed the
  "/challenge/run" program

```
hacker@paths~position-thy-self:~$ cd /challenge/run
bash: cd: /challenge/run: Not a directory
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/share/build-essential directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usr/share/build-essential
hacker@paths~position-thy-self:/usr/share/build-essential$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{EvbWmXqBtOn77r2Hvsd1fjuwZIc.QX2QTN0wiN3gjNzEzW}
```

Incorrect Tangents :
Accidentally used cd on /challenge/run even though its not a directory and is a program inside the given directory in the challenge

References :
None
