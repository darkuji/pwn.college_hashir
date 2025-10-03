# Killing Processes
### The challenge asks us to terminate a process


## My Solve
**Flag:** pwn.college{Mf-i2LapS0bBxkSEd2ndjLTSBB8.QXyQDO0wSO1EzNzEzW}
Used ps -ef to list out all the running processes where i found the 
id of the dont_run process. Used kill command to end the process 
after which i ran /challenge/run to get the flag


```
hacker@processes~killing-processes:~$ ps -ef
UID          PID    PPID  C STIME TTY          TIME CMD
root           1       0  0 15:30 ?        00:00:00 /sbin/docker-init -- /nix/var/nix/profiles/dojo-workspace/bin/dojo-i
root           7       1  0 15:30 ?        00:00:00 /run/dojo/bin/sleep 6h
root         135       1  0 15:30 ?        00:00:00 su -c /challenge/.launcher hacker
hacker       136     135  0 15:30 ?        00:00:00 /challenge/dont_run
hacker       137     136  0 15:30 ?        00:00:00 sleep 6h
hacker       139       0  0 15:30 pts/0    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       145       0  0 15:30 pts/1    00:00:00 /nix/store/0nxvi9r5ymdlr2p24rjj9qzyms72zld1-bash-interactive-5.2p37/
hacker       151     139  0 15:30 pts/0    00:00:00 /run/dojo/bin/bash --login
hacker       158     145  0 15:30 pts/1    00:00:00 /run/dojo/bin/bash --login
hacker       170     151  0 15:30 pts/0    00:00:00 ps -ef
hacker@processes~killing-processes:~$ kill 136
hacker@processes~killing-processes:~$ /challenge/run
Great job! Here is your payment:
pwn.college{Mf-i2LapS0bBxkSEd2ndjLTSBB8.QXyQDO0wSO1EzNzEzW}
```

## What I Learned
I learned how we can use the kill command to terminate an ongoing process

## References
None