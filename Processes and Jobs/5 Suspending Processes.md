# Suspending Processes
### The challenge asks us to suspend a process


## My Solve
**Flag:** pwn.college{sRI8Rwfz8YWHVjXyEHOOP9FKWtW.QX1QDO0wSO1EzNzEzW}
Used /challenge/run then used Ctrl Z to suspend the process then used
/challenge/run again and it detected that another copy was running and
gave me the flag


```
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         154     135  0 16:53 pts/0    00:00:00 bash /challenge/run
root         156     154  0 16:53 pts/0    00:00:00 ps -f

I don't see a second me!

To pass this level, you need to suspend me and launch me again! You can
background me with Ctrl-Z or, if you're not ready to do that for whatever
reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~suspending-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running in
this terminal... Let's check!

UID          PID    PPID  C STIME TTY          TIME CMD
root         154     135  0 16:53 pts/0    00:00:00 bash /challenge/run
root         161     135  0 16:53 pts/0    00:00:00 bash /challenge/run
root         163     161  0 16:53 pts/0    00:00:00 ps -f

Yay, I found another version of me! Here is the flag:
pwn.college{sRI8Rwfz8YWHVjXyEHOOP9FKWtW.QX1QDO0wSO1EzNzEzW}
```

## What I Learned
Learned how to suspend a process 

## References
None