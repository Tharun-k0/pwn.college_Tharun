# Challenge 7 : Exclusionary Globbing

Developed an understanding of using different globs in a single argument

## My solve

**Flag:** pwn.college{Ylal9pmuAcXk0EpTC9f6wYqS-wK.QX2IDO0wiN3gjNzEzW}

What I Learnt: How to use multiple different globs in a single arguument

- As the challenge asked I cded to /challenge/files directory and used both bracket-glob and _ in the argument as I observed that no other file was starting with the same letters as the ones we needed so i used [cep]_ to include all the required files and get the flag.

```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]
Your expansion did not expand to the requested files (amazing beautiful
challenging delightful educational fantastic great happy incredible jovial kind
laughing magical optimistic queenly radiant splendid thrilling uplifting
victorious xenial youthful zesty).
Instead, it expanded to:
[!pwn]
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [^pwn]
Your expansion did not expand to the requested files (amazing beautiful
challenging delightful educational fantastic great happy incredible jovial kind
laughing magical optimistic queenly radiant splendid thrilling uplifting
victorious xenial youthful zesty).
Instead, it expanded to:
[^pwn]
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{Ylal9pmuAcXk0EpTC9f6wYqS-wK.QX2IDO0wiN3gjNzEzW}
```

Incorrect Tangents :
Didnt put \* after the bracket glob resulting in only matching single characters and not excluding whole filenames.

References :
None
