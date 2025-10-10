# The SUID Bit
### The challenge asks us to add SUID bit to get root access


## My Solve
**Flag:** pwn.college{kjMGOU2oOrDTujICJwjrjdXN6qQ.QXzEjN0wSO1EzNzEzW}
Used chmod u+s /challenge/getroot to set the files SUID then used
the program to get access to root and catted the flag


```
hacker@permissions~the-suid-bit:~$ chmod u+s /challenge/getroot
hacker@permissions~the-suid-bit:~$ /challenge/getroot
SUCCESS! You have set the suid bit on this program, and it is running as root!
Here is your shell...
root@permissions~the-suid-bit:~# cat /flag
pwn.college{kjMGOU2oOrDTujICJwjrjdXN6qQ.QXzEjN0wSO1EzNzEzW}
```

## What I Learned
Learned how to add SUID bit to  spawn a root shell

## References
None