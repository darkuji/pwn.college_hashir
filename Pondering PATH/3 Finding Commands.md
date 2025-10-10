# Finding Commands
### The challenge asks us to find where a command is located


## My Solve
**Flag:** pwn.college{wgSaWj4MpDn5mFNx9odYl5USTFB.01NzEzNxwSO1EzNzEzW}
Used find win to get the path of the win command then catted the flag
which was in the same folder

```
hacker@path~finding-commands:~$ which win
/challenge/paths/28996/win
hacker@path~finding-commands:~$ cat /challenge/paths/28996/flag
pwn.college{wgSaWj4MpDn5mFNx9odYl5USTFB.01NzEzNxwSO1EzNzEzW}
```

## What I Learned
Learned how to find where a command is located using the which command

## References
None