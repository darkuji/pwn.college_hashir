# Making Directories
### The challenge asks us to create our own directory and add a new file to it


## My Solve
**Flag:** pwn.college{EV8kaj5YiYWaZ6STw-Kj80NHdAg.QXxMDO0wSO1EzNzEzW}
I first changed my cwd to /tmp before using the mkdir command to
create my own directory named pwn after which i used ls to make
sure it was created successfully after  which i changed the cwd
to pwn before using the touch command to create a new file named
college and running the /challenge/run command


```
hacker@commands~making-directories:~$ cd /tmp
hacker@commands~making-directories:/tmp$ mkdir pwn
hacker@commands~making-directories:/tmp$ ls
bin  hsperfdata_root  pwn  tmp.TpSOPGOVKK
hacker@commands~making-directories:/tmp$ cd /tmp/pwn
hacker@commands~making-directories:/tmp/pwn$ touch college
hacker@commands~making-directories:/tmp/pwn$ /challenge/run
Success! Here is your flag:
pwn.college{EV8kaj5YiYWaZ6STw-Kj80NHdAg.QXxMDO0wSO1EzNzEzW}
```

## What I Learned
I learned how to create new directories in a Linux environment 
using the mkdir command 

## References
None