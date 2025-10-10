# Changing file ownership
### The challenge asks us to change the ownership rights of a file


## My Solve
**Flag:** pwn.college{AoZqfZSnb8_neP1yIZbzzNLHxdR.QXxEjN0wSO1EzNzEzW}
Used the chown hacker /flag command to change the owner of /flag
file to hacker then catted the file


```
hacker@permissions~changing-file-ownership:~$ chown hacker /flag
hacker@permissions~changing-file-ownership:~$ cat /flag
pwn.college{AoZqfZSnb8_neP1yIZbzzNLHxdR.QXxEjN0wSO1EzNzEzW}
```

## What I Learned
I learned how to use the chown command which is basically used to
change the owner of a file by taking the username and file name 
as its arguments

## References
None