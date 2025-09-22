# Paths Position Elsewhere
### The challenge asks us to change the working directory to a new one in order to access a program


## My Solve
**Flag:** pwn.college{8yuh8TJtIrB-5yhziOXbtnt0H3s.QX3QTN0wSO1EzNzEzW}

I first tried to run the /challenge/run command to know if i was in the 
right working directory which i wasn't. Then i used the cd command to 
enter into the /var directory and then run /challenge/run command
to obtain the flag



```
hacker@paths~position-elsewhere:~$ /challenge/run
Incorrect...
You are not currently in the /var directory.
Please use the `cd` utility to change directory appropriately.
hacker@paths~position-elsewhere:~$ cd /var
hacker@paths~position-elsewhere:/var$ /challenge/run
Correct!!!
/challenge/run is an absolute path, invoked from the right directory!
Here is your flag:
pwn.college{8yuh8TJtIrB-5yhziOXbtnt0H3s.QX3QTN0wSO1EzNzEzW}
```

## What I Learned
I learned how to use the cd command to change the working directory of 
the Linux environment to access new directories and programs within it


## References

