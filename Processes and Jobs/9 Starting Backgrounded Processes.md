# Starting Backgrounded Processes
### The challenge asks us to start a backgrounded process


## My Solve
**Flag:** pwn.college{IaPgF6i1LBwur5Jxe3C1d9EUbBY.QX5QDO0wSO1EzNzEzW}
Used /challenge/run &bg to make it run in the background coz sleep
was already running to obtain the flag


```
hacker@processes~starting-backgrounded-processes:~$ /challenge/run &bg
[1] 146
bash: bg: job 1 already in background
hacker@processes~starting-backgrounded-processes:~$


Yay, you started me in the background! Because of that, this text will probably
overlap weirdly with the shell prompt, but you're used to that by now...

Anyways! Here is your flag!
pwn.college{IaPgF6i1LBwur5Jxe3C1d9EUbBY.QX5QDO0wSO1EzNzEzW}
```

## What I Learned
I learned how to run a process that has been backgrounded using &bg command

## References
None