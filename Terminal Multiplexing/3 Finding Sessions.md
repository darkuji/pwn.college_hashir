# Finding Sessions
### The challenge asks us to find screen sessions


## My Solve
**Flag:** pwn.college{Iywkekv7_3FZo14tRTOk1cYdtiE.01N4IDOxwSO1EzNzEzW}
Used screen -ls to see all the active sessions then launched all of them
using screen -r screenname then got the flag in the last one 


```
hacker@terminal-multiplexing~finding-sessions:~$  echo 'Congratulations! You found the right session!'
Congratulations! You found the right session!
hacker@terminal-multiplexing~finding-sessions:~$  echo pwn.college{Iywkekv7_3FZo14tRTOk1cYdtiE.01N4IDOxwSO1EzNzEzW}
pwn.college{Iywkekv7_3FZo14tRTOk1cYdtiE.01N4IDOxwSO1EzNzEzW}


hacker@terminal-multiplexing~finding-sessions:~$ screen -ls
There are screens on:
        150.pts-0.terminal-multiplexing~launching-screen        (Remote or dead)
        139.pts-0.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        140.pts-0.terminal-multiplexing~detaching-and-attaching (Remote or dead)
        144.session_1211384fc1de1608    (Detached)
        147.session_0122164ed046bf2c    (Detached)
        150.session_b241aac08870af61    (Detached)
6 Sockets in /home/hacker/.screen.
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_1211384fc1de1608
[detached from 144.session_1211384fc1de1608]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_0122164ed046bf2c
[detached from 147.session_0122164ed046bf2c]
hacker@terminal-multiplexing~finding-sessions:~$ screen -r session_b241aac08870af61
[detached from 150.session_b241aac08870af61]
```

## What I Learned
I learned how to view the active screen sessions using screen -ls

## References
None