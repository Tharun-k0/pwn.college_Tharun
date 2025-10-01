# Challenge 5 : Multiple Globs

Developed an understanding of using multiple globs in a single argument

## My solve

**Flag:** pwn.college{IF9jToPyHqvTcdphYh4DnzrmVAt.0lM3kjNxwiN3gjNzEzW}

What I Learnt: How to use multiple \* globs in a single arguument

- As the challenge asked I cded to /challenge/files directory and used two \*'s in the argument to run /challenge/run so that it covers every word having the letter p in it to get the flag

```
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ ls
amazing    challenging  educational  great  incredible  kind      magical  optimistic  queenly  splendid   uplifting   wonderful  youthful
beautiful  delightful   fantastic    happy  jovial      laughing  nice     pwning      radiant  thrilling  victorious  xenial     zesty
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{IF9jToPyHqvTcdphYh4DnzrmVAt.0lM3kjNxwiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
