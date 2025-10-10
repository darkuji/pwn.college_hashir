# Fun with group names
### The challenge asks us to change the group owner of a file


## My Solve
**Flag:** pwn.college{cc2TihVf4E8fAzqfzyPWAyD-s_h.QXycjM1wSO1EzNzEzW}
Used id to list out all the group names then used chgrp grp10053 /flag
to change the group owner of /flag to grp10053 then catted the flag


```
hacker@permissions~fun-with-groups-names:~$ id
uid=1000(hacker) gid=1000(grp10053) groups=1000(grp10053)
hacker@permissions~fun-with-groups-names:~$ chgrp grp10053 /flag
hacker@permissions~fun-with-groups-names:~$ cat /flag
pwn.college{cc2TihVf4E8fAzqfzyPWAyD-s_h.QXycjM1wSO1EzNzEzW}
```

## What I Learned
I learned how to change the group owner of a file


## References
None