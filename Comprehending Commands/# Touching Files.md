# Touching Files
### The challenge asks us to create a new file using the touch command


## My Solve
**Flag:** pwn.college{AaPkMKz333hYLqhl5lBCEvOGLzU.QXwMDO0wSO1EzNzEzW}
I first changed my cwd to /temp then i used the touch command twice to
create new files namely college and pwn then i used the ls command 
to make sure that my files were created successfully and then i u


```
hacker@commands~touching-files:~$ cd /tmp
hacker@commands~touching-files:/tmp$ touch college
hacker@commands~touching-files:/tmp$ touch pwn
hacker@commands~touching-files:/tmp$ ls
bin  college  hsperfdata_root  pwn  tmp.TpSOPGOVKK
hacker@commands~touching-files:/tmp$ /challenge/run
Success! Here is your flag:
pwn.college{AaPkMKz333hYLqhl5lBCEvOGLzU.QXwMDO0wSO1EzNzEzW}
```

## What I Learned
I learned how to create new files in a Linux environment using the
touch command by just giving the names of the new files as arguments

## References
None