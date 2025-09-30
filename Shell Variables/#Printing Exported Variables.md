# Printing Exported Variables
### The challenge asks us to print exported variables using env


## My Solve
**Flag:** pwn.college{wj-CDj4OvlccJH3KpLnx9qkdBVQ.QX4UTN0wSO1EzNzEzW}
ran env to get a list of exported variables


```
hacker@variables~printing-exported-variables:~$ env
SHELL=/run/dojo/bin/bash
HOSTNAME=variables~printing-exported-variables
PWD=/home/hacker
MANPATH=/run/dojo/share/man:
DOJO_AUTH_TOKEN=ea38ee0ecc645ed5c2ab652e33429355c9c873c76b166b3ca1d7ebd998bc52c9
HOME=/home/hacker
LANG=C.UTF-8
FLAG=pwn.college{wj-CDj4OvlccJH3KpLnx9qkdBVQ.QX4UTN0wSO1EzNzEzW}
TERMINFO=/run/dojo/share/terminfo
TERM=xterm-256color
SHLVL=2
LC_CTYPE=C.UTF-8
SSL_CERT_FILE=/run/dojo/etc/ssl/certs/ca-bundle.crt
PATH=/run/challenge/bin:/run/dojo/bin:/root/.cargo/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
DEBIAN_FRONTEND=noninteractive
_=/run/dojo/bin/env
```

## What I Learned
Learned how to print the list of exported variables

## References
None