# Named Pipes
### The challenge asks us to work with FIFO files


## My Solve
**Flag:** pwn.college{4fm2l22-MYL-V00FQJeT9UFxDNA.01MzMDOxwSO1EzNzEzW}
I first created a fifo file and redirected the output of /challenge/run
to the file after which i 


```
hacker@piping~named-pipes:~$ mkfifo /tmp/flag_fifo
hacker@piping~named-pipes:~$ /challenge/run >> /tmp/flag_fifo
You're successfully redirecting /challenge/run to a FIFO at /tmp/flag_fifo!
Bash will now try to open the FIFO for writing, to pass it as the stdout of
/challenge/run. Recall that operations on FIFOs will *block* until both the
read side and the write side is open, so /challenge/run will not actually be
launched until you start reading from the FIFO!
cat /tmp/flag_fifo
hacker@piping~named-pipes:~$ cat /tmp/flag_fifo
You've correctly redirected /challenge/run's stdout to a FIFO at
/tmp/flag_fifo! Here is your flag:
pwn.college{4fm2l22-MYL-V00FQJeT9UFxDNA.01MzMDOxwSO1EzNzEzW}
```

## What I Learned
I learned about fifo files and how we need to read and write them at the 
same time


## References
None