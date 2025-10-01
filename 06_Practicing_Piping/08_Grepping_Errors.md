# Challenge 8 : Grepping Errors

Developed an understanding of grepping errors using the >& operator along with |

## My solve

**Flag:** pwn.college{81nbr8srtQv09naOQP0Ti7bWt_I.QX1ATO0wiN3gjNzEzW}

What I Learnt: How to use >& operator to redirect errors along with stdout to grep both simultaneously

- As the challenge asked I used >& to redirect stderr onto stdout and then use the | operator with grep to get the flag

```
hacker@piping~grepping-errors:~$ /challenge/run 2>& 1
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...

[FAIL] You did not satisfy all the execution requirements.
[FAIL] Specifically, you must fix the following issue:
[FAIL]   stderr of this process does not appear to be a pipe!
hacker@piping~grepping-errors:~$ /challenge/run 2>& 1 | grep pwn.college
[INFO] WELCOME! This challenge makes the following asks of you:
[INFO] - the challenge checks for a specific process at the other end of stderr : grep
[INFO] - the challenge will output a reward file if all the tests pass : /challenge/.data.txt

[HYPE] ONWARDS TO GREATNESS!

[INFO] This challenge will perform a bunch of checks.
[INFO] If you pass these checks, you will receive the /challenge/.data.txt file.

[TEST] You should have redirected my stderr to another process. Checking...
[TEST] Performing checks on that process!

[INFO] The process' executable is /nix/store/8b4vn1iyn6kqiisjvlmv67d1c0p3j6wj-gnugrep-3.11/bin/grep.
[INFO] This might be different than expected because of symbolic links (for example, from /usr/bin/python to /usr/bin/python3 to /usr/bin/python3.8).
[INFO] To pass the checks, the executable must be grep.

[PASS] You have passed the checks on the process on the other end of my stderr!
[PASS] Success! You have satisfied all execution requirements.
pwn.college{81nbr8srtQv09naOQP0Ti7bWt_I.QX1ATO0wiN3gjNzEzW}
```

Incorrect Tangents :
Since in the challenge it mentioned a two step process i thought i had to use >& operator first then seperately use the | and grep but it showed an error and worked when i tried doing it together

References :
None
