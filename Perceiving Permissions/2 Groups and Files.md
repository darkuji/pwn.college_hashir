# Groups and Files
### The file asks us to change the group ownership of a file


## My Solve
**Flag:** pwn.college{oetEkJm4VoZuTczcIlHB-cv-i2M.QXxcjM1wSO1EzNzEzW}
Used chgrp hacker /flag to change the owner group of /flag to hacker
then ran cat /flag to read it


```
hacker@permissions~groups-and-files:~$ chgrp hacker /flag
hacker@permissions~groups-and-files:~$ cat /flag
pwn.college{oetEkJm4VoZuTczcIlHB-cv-i2M.QXxcjM1wSO1EzNzEzW}
```

## What I Learned
I learned how users can belong to groups that have access to a file
and in order to change the group which owns the file we can use the 
chgrp command with the arguments as the new owner name and the file name

## References
None