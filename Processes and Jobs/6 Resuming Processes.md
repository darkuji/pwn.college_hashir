# Resuming Processes
### The challenge asks us to suspend a process then resume it


## My Solve
**Flag:** pwn.college{oYveGOTunvWaYMSyP4P9XCcTkmX.QX2QDO0wSO1EzNzEzW}
Used /challenge/run and used Ctrl Z to suspend it then used fg to
resume it and obtained the flag


```
hacker@processes~resuming-processes:~$ /challenge/run
Let's practice resuming processes! Suspend me with Ctrl-Z, then resume me with
the 'fg' command! Or just press Enter to quit me!
^Z
[2]+  Stopped                 /challenge/run
hacker@processes~resuming-processes:~$ fg
/challenge/run
I'm back! Here's your flag:
pwn.college{oYveGOTunvWaYMSyP4P9XCcTkmX.QX2QDO0wSO1EzNzEzW}
Don't forget to press Enter to quit me!
```

## What I Learned
Learned how to resume a process using fg command

## References
None