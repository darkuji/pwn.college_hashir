\# Listing Processes

\### The challenge asks us to list processes going on in the environment





\## My Solve

\*\*Flag:\*\* pwn.college{cowgBJTaot2Q047h3-4Y1NiuvGq.QX4MDO0wSO1EzNzEzW}

Used ps -ef to list the processes going on in the environment where

i found that /challenge/run had been renamed to /challenge/11607-run-12989

executed the file and obtained the flag





```

hacker@processes~listing-processes:~$ ps -ef

UID          PID    PPID  C STIME TTY          TIME CMD

root           1       0  0 15:17 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i

root           7       1  0 15:17 ?        00:00:00 /run/dojo/bin/sleep 6h

root         132       1  0 15:17 ?        00:00:00 /challenge/11607-run-12989

root         135     132  0 15:17 ?        00:00:00 sleep 6h

hacker       137       0  0 15:17 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/

hacker       143     137  0 15:17 pts/0    00:00:00 /run/dojo/bin/bash --login

hacker       152       0  0 15:18 pts/1    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/

hacker       158     152  0 15:18 pts/1    00:00:00 /run/dojo/bin/bash --login

hacker       168     158  0 15:26 pts/1    00:00:00 ps -ef

hacker@processes~listing-processes:~$ /challenge/11607-run-12989

Yahaha, you found me! Here is your flag:

pwn.college{cowgBJTaot2Q047h3-4Y1NiuvGq.QX4MDO0wSO1EzNzEzW}

Now I will sleep for a while (so that you could find me with 'ps').

```



\## What I Learned
I learned how we can list out the different processes that are going on in the environment



\## References

None

