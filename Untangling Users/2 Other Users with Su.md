# Other Users with Su
### The challenge asks us to become other users with su 


## My Solve
**Flag:** pwn.college{gm3RmFd7MkJMFQ8q7aFUAie0rDN.QX2UDN1wSO1EzNzEzW}
Used su zardus to become the user zardus then entered password to 
gain access to files then ran /challenge/run to obtain the flag

```
hacker@users~other-users-with-su:~$ su zardus
Password:
zardus@users~other-users-with-su:/home/hacker$ cat /flag
cat: /flag: Permission denied
zardus@users~other-users-with-su:/home/hacker$ /challenge/run
Congratulations, you have become Zardus! Here is your flag:
pwn.college{gm3RmFd7MkJMFQ8q7aFUAie0rDN.QX2UDN1wSO1EzNzEzW}
```

## What I Learned
Learned how to become another user using the su command
and giving the username as the argument

## References
None