# Foregrounding Processes
### The challenge asks us to foreground a process


## My Solve
**Flag:** pwn.college{QhbzWnojhbl6o6N6s3qYYl5cDns.QX4QDO0wSO1EzNzEzW}
Used /challenge/run and Ctrl Z to suspend the process then bg to make
it run in the background and fg to make it run in the foreground and obtained
the flag


```
hacker@processes~foregrounding-processes:~$ /challenge/run
To pass this level, you need to suspend me, resume the suspended process in the
background, and *then* foreground it without re-suspending it! You can
background me with Ctrl-Z (and resume me in the background with 'bg') or, if
you're not ready to do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~foregrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~foregrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out. After that, resume me into the foreground with 'fg';
I'll wait.
fg
/challenge/run
YES! Great job! I'm now running in the foreground. Hit Enter for your flag!

pwn.college{QhbzWnojhbl6o6N6s3qYYl5cDns.QX4QDO0wSO1EzNzEzW}
```

## What I Learned
I learned how to make a backgrounded process run in the foreground so that
it can be operated on to some extent

## References
None