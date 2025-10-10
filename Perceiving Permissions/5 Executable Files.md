# Executable Files
### The challenge asks us to change permissions so taht a file can be executed


## My Solve
**Flag:** pwn.college{8c1MP0igKSjbjvbibilcwuFbsp-.QXyEjN0wSO1EzNzEzW}
Used chmod a+x /challenge/run so that the program can be executed by 
all users then executed the program


```
hacker@permissions~executable-files:~$ chmod o-x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
bash: /challenge/run: Permission denied
hacker@permissions~executable-files:~$ chmod a+x /challenge/run
hacker@permissions~executable-files:~$ /challenge/run
Successful execution! Here is your flag:
pwn.college{8c1MP0igKSjbjvbibilcwuFbsp-.QXyEjN0wSO1EzNzEzW}
```

## What I Learned
I learned how to give permission to execute a file and the difference
between reading and execution

## References
None