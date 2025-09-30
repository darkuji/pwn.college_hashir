# Redirecting Errors
### The challenge asks us to redirect the errors that may be present to a different file


## My Solve
**Flag:** pwn.college{IaJjAcu2maUCrfub28aRwJPqQIh.QX3YTN0wSO1EzNzEzW}
I used the /challenge/run > myflag to redirect the output of the 
program to the myflag file. Further i used the 2> instructions part
so that all the errors that may be present in the file get redirected
to the instructions file


```
hacker@piping~redirecting-errors:~$ /challenge/run > myflag 2> instructions
hacker@piping~redirecting-errors:~$ cat myflag

[FLAG] Here is your flag:
[FLAG] pwn.college{IaJjAcu2maUCrfub28aRwJPqQIh.QX3YTN0wSO1EzNzEzW}
```

## What I Learned
I learned how we can separately redirect output and errors in a program
to different files using different forms of >

## References
None