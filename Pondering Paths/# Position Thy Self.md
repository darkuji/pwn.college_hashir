# Position Thy Self
### The challenge asks us to change the current working directory to a new one and then enter into a program's absolute path to obtain the flag


## My Solve
**Flag:** pwn.college{Q08MCaiBeXVbpohIi2xrTVxK39Q.QX2QTN0wSO1EzNzEzW}

I first tried to run the /challenge/run command to know if i was in the 
right working directory which i wasn't. Then i used the cd command to 
enter into the /usr/bin directory and then run /challenge/run command
to obtain the flag



```
hacker@paths~position-thy-self:~$ /challenge/run
Incorrect...
You are not currently in the /usr/bin directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-thy-self:~$ cd /usr/bin
hacker@paths~position-thy-self:/usr/bin$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Q08MCaiBeXVbpohIi2xrTVxK39Q.QX2QTN0wSO1EzNzEzW}
```

## What I Learned
I learned how to use the cd command to change the working directory of 
the Linux environment to access new directories and programs within it



## References

None
