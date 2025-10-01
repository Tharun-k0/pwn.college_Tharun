# Challenge 3 : Matching With []

Developed an understanding of third glob []

## My solve

**Flag:** pwn.college{o_L7Lw-IyNe5Du7oNYHFFAUNOHV.QXzIDO0wiN3gjNzEzW}

What I Learnt: Understood how to use the [] glob

- cded to the /challenge/files directory and used the bracket-glob with /challenge/run to only get the required files and get the flag

```
hacker@globbing~matching-with-:~$ cd /challenge/files
hacker@globbing~matching-with-:/challenge/files$ ls
file_a  file_c  file_e  file_g  file_i  file_k  file_m  file_o  file_q  file_s  file_u  file_w  file_y
file_b  file_d  file_f  file_h  file_j  file_l  file_n  file_p  file_r  file_t  file_v  file_x  file_z
hacker@globbing~matching-with-:/challenge/files$ /challenge/run file_[bash]
You got it! Here is your flag!
pwn.college{o_L7Lw-IyNe5Du7oNYHFFAUNOHV.QXzIDO0wiN3gjNzEzW}
```

Incorrect Tangents :
None

References :
None
