# Challenge 11 : Process Substitution For Input

Developed an understanding of comparing the outputs of two commands

## My solve

**Flag:** pwn.college{waLR6bm0u7LxKnZ3EPsk1fLzwNq.0lNwMDOxwiN3gjNzEzW}

What I Learnt: How to use <(command) to get the output of command

- Used <(command) to get the output of both commands and diff together with it to print out the real flag from the mixture of flags and decoys as told in the challenge

```
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
98a99
> pwn.college{waLR6bm0u7LxKnZ3EPsk1fLzwNq.0lNwMDOxwiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
