# Challenge 9 : Multiple Options For Tab Completion

Developed an understanding of tab completion when there are multiple options

## My solve

**Flag:** pwn.college{w4t6mikLEs8kRVfPFuD9065aQPl.0lN0EzNxwiN3gjNzEzW}

What I Learnt: How to use tab completion when there are multiple options

- As the challenge asked I used tab completion to list out all possible files and then go through them to find out the file containing the flag

```
hacker@globbing~multiple-options-for-tab-completion:~$ /challenge/files/pwn
pwn                    pwn-the-planet         pwncollege-flamingo    pwncollege-hacking
pwn-college            pwncollege-family      pwncollege-flyswatter
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn-college
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwn-the-planet
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-family
No flag in this file!
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-fla
pwncollege-flag      pwncollege-flamingo
hacker@globbing~multiple-options-for-tab-completion:~$ cat /challenge/files/pwncollege-flag
pwn.college{w4t6mikLEs8kRVfPFuD9065aQPl.0lN0EzNxwiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
