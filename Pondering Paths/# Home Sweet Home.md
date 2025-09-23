# Home Sweet Home
### The challenge asks us to use the relative path with a file as an argument


## My Solve
**Flag:**pwn.college{kDHPFlgBtHRd35QYm_VcRiGuEJe.QXzMDO0wSO1EzNzEzW}
I first changed the directory to home using the 'cd' command then i used the 
/challenge/run command with the argument as /a which is the file in which
my flag would be written and stored



```
hacker@paths~home-sweet-home:$ cd /home
hacker@paths~home-sweet-home:/home$ /challenge/run ~/a
Writing the file to /home/hacker/a!
... and reading it back to you:
pwn.college{kDHPFlgBtHRd35QYm_VcRiGuEJe.QXzMDO0wSO1EzNzEzW}
```

## What I Learned
I learned how to give a file path as an argument while providing a relative 
path in a Linux environment


## References
None