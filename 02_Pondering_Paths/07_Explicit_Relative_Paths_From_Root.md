# Challenge 7 : Explicit Relative Paths, From /

Had to navigate to root dir and then call challenge/run using relative path

## My solve

**Flag:** pwn.college{kWkmPdy40uK9wbUXvXuYG43n2MT.QXwUTN0wiN3gjNzEzW}

What I Learnt: Invoking programs using explicit relative paths from the root directory

-I used cd to go into the root directory and then invoked challenge/run

```
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{kWkmPdy40uK9wbUXvXuYG43n2MT.QXwUTN0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
