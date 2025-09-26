# Position yet Elsewhere
### The challenge asks us to change the working directory to a new one in order to access a program


## My Solve
**Flag:** pwn.college{Q1TUMjwA-rYUo6GdJtCipFFNah_.QX4QTN0wSO1EzNzEzW}
I first tried to run the /challenge/run command to know if i was in the 
right working directory which i wasn't. Then i used the cd command to 
enter into the /var/log directory and then run /challenge/run command
to obtain the flag



```
hacker@paths~position-yet-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /var/log directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-yet-elsewhere:~$ cd /var/log
hacker@paths~position-yet-elsewhere:/var/log$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{Q1TUMjwA-rYUo6GdJtCipFFNah_.QX4QTN0wSO1EzNzEzW}
```

## What I Learned
I learned how to use the cd command to change the working directory of 
the Linux environment to access new directories and programs within it


## References

None