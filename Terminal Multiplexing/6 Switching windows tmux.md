# Switching windows tmux
### The challenge asks us to switch windows in tmux


## My Solve
**Flag:** pwn.college{U3xVyrIGeGAcvfTaQ3DsDWUj5uE.0FM5IDOxwSO1EzNzEzW}
Used tmux a to open the tmux then ctrl b 0 to go to window 0 and got the flag


```
hacker@terminal-multiplexing~switching-windows-tmux:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{U3xVyrIGeGAcvfTaQ3DsDWUj5uE.0FM5IDOxwSO1EzNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{U3xVyrIGeGAcvfTaQ3DsDWUj5uE.0FM5IDOxwSO1EzNzEzW}

hacker@terminal-multiplexing~switching-windows-tmux:~$ tmux a
```

## What I Learned
I learned how to switch windows in tmux

## References
None