# Challenge 5 : Printing Exported Variables

Developed an understanding of how to print exported variables

## My solve

**Flag:** pwn.college{Qmbl3ZAll9MzS7VTPr7m5OiD92y.QX4UTN0wiN3gjNzEzW}

What I Learnt: How to print exported variables using env command

- As told in the challenge I just used the env command to print out the values of exported variables

```
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=eb6252c4c4966ab6520e2581388df7f9bf7844b5ac57e882cbe10adc53b221e7
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{Qmbl3ZAll9MzS7VTPr7m5OiD92y.QX4UTN0wiN3gjNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

Incorrect Tangents :
None

References :
None
