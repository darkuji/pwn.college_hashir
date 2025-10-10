# Switching Windows
### The challenge asks us to switch windwows


## My Solve
**Flag:** pwn.college{UMZLygrj45zCh0DCjlW8is7Cr6g.0FO4IDOxwSO1EzNzEzW}
Used screen -r to open the screen then pressed ctrl A and 0 to go to 
window 0 and got the flag


```
hacker@terminal-multiplexing~switching-windows:~$  cat <<MSG
> Excellent work! You found window 0!
> Here is your flag: pwn.college{UMZLygrj45zCh0DCjlW8is7Cr6g.0FO4IDOxwSO1EzNzEzW}
> MSG
Excellent work! You found window 0!
Here is your flag: pwn.college{UMZLygrj45zCh0DCjlW8is7Cr6g.0FO4IDOxwSO1EzNzEzW}

hacker@terminal-multiplexing~switching-windows:~$ screen -r
```

## What I Learned
Learned how to switch windows

## References
None