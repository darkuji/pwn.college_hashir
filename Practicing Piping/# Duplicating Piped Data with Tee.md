# Duplicating Piped Data with Tee
### Challenge asks us to use tee command to debug command output


## My Solve
**Flag:** pwn.college{4_TpuBnXLjy8ozdL5MPEd8jUJDq.QXxITO0wSO1EzNzEzW}
Ran the commands to store input in two files and obtained the flag


```
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn | tee flag | /challenge/college
Processing...
WARNING: you are overwriting file flag with tee's output...
The input to 'college' does not contain the correct secret code! This code
should be provided by the 'pwn' command. HINT: use 'tee' to intercept the
output of 'pwn' and figure out what the code needs to be.
hacker@piping~duplicating-piped-data-with-tee:~$ cat flag
Usage: /challenge/pwn --secret [SECRET_ARG]

SECRET_ARG should be "4_TpuBnX"
hacker@piping~duplicating-piped-data-with-tee:~$ /challenge/pwn --secret 4_TpuBnX | tee flag | /challenge/college
Processing...
WARNING: you are overwriting file flag with tee's output...
Correct! Passing secret value to /challenge/college...
Great job! Here is your flag:
pwn.college{4_TpuBnXLjy8ozdL5MPEd8jUJDq.QXxITO0wSO1EzNzEzW}
```

## What I Learnt
Tee can be used with | to debug the input being sent to a command

## References
None