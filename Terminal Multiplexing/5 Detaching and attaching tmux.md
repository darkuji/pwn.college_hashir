# Detaching and attaching tmux
### The challenge asks us to attach and detach tmux


## My Solve
**Flag:** pwn.college{Q1hFUhiU8S97C5mahV8F4gGghk9.0VO4IDOxwSO1EzNzEzW}
Used tmux to open tmux then ctrl b d to detach it then ran /challenge/run
then used tmux attach to go to the tmux again and got the flag


```
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$  echo Congratulations, here is your flag: pwn.college{Q1hFUhiU8S97C5mahV8F4gGghk9.0VO4IDOxwSO1EzNzEzW}
Congratulations, here is your flag: pwn.college{Q1hFUhiU8S97C5mahV8F4gGghk9.0VO4IDOxwSO1EzNzEzW}

tmuxhacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux
[detached (from session 0)]
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ /challenge/run
Found detached tmux session: 0
Sending flag to your tmux session...

Flag sent! Now reattach to your tmux session with:
  tmux attach

You'll find the flag waiting for you there!
hacker@terminal-multiplexing~detaching-and-attaching-tmux:~$ tmux attach
```

## What I Learned
I learned what a tmux is and how to attach and detach a tmux

## References
None