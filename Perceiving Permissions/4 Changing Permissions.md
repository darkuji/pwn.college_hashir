# Changing Permissions
### The challenge asks us to change the permissions of a file


## My Solve
**Flag:** pwn.college{4mbSZJV1Tm9nM7h8l6O_f3RN1xa.QXzcjM1wSO1EzNzEzW}
Used chmod a+r/flag to change the permissions of /flag so that all users
can read it then catted the flag


```
hacker@permissions~changing-permissions:~$ chmod a+r /flag
hacker@permissions~changing-permissions:~$ cat /flag
pwn.college{4mbSZJV1Tm9nM7h8l6O_f3RN1xa.QXzcjM1wSO1EzNzEzW}
```

## What I Learned
Learned how to change the permissions of a file

## References
None