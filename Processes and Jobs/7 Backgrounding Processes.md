# Backgrounding Processes
### The challenge asks us to background a process without terminating it


## My Solve
**Flag:** pwn.college{MKa3xlwmcwnyoKxwItKuTRLHXb1.QX3QDO0wSO1EzNzEzW}
Used /challenge/run then Ctrl Z to suspend it then used bg to keep it
running in the background and then i used /challenge/run to start another
copy with which i got the flag


```
hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         139 S+   bash /challenge/run
root         141 R+   ps -o user=UID,pid,stat,cmd

I don't see a second me!

To pass this level, you need to suspend me, resume the suspended process in the
background, and then launch a new version of me! You can background me with
Ctrl-Z (and resume me in the background with 'bg') or, if you're not ready to
do that for whatever reason, just hit Enter and I'll exit!
^Z
[1]+  Stopped                 /challenge/run
hacker@processes~backgrounding-processes:~$ bg
[1]+ /challenge/run &
hacker@processes~backgrounding-processes:~$


Yay, I'm now running the background! Because of that, this text will probably
overlap weirdly with the shell prompt. Don't panic; just hit Enter a few times
to scroll this text out.

hacker@processes~backgrounding-processes:~$ /challenge/run
I'll only give you the flag if there's already another copy of me running *and
not suspended* in this terminal... Let's check!

UID          PID STAT CMD
root         139 S    bash /challenge/run
root         149 S    sleep 6h
root         150 S+   bash /challenge/run
root         152 R+   ps -o user=UID,pid,stat,cmd

Yay, I found another version of me running in the background! Here is the flag:
pwn.college{MKa3xlwmcwnyoKxwItKuTRLHXb1.QX3QDO0wSO1EzNzEzW}
```

## What I Learned
I learned how to background an ongoing process in a Linux environment

## References
None