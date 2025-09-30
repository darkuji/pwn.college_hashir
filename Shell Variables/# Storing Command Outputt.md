# Storing Command Output
### The challenge asks us to directly assign a variable to a command output


## My Solve
**Flag:** pwn.college{YWdnQlvfw1andSHi6tqZta0lcUT.QX1cDN1wSO1EzNzEzW}
Used PWN=$(cat /challenge/run) to assign the flag to PWN then printed 
the PWN variable


```
hacker@variables~storing-command-output:~$ PWN=$(cat /challenge/run)
hacker@variables~storing-command-output:~$ PWN
bash: PWN: command not found
hacker@variables~storing-command-output:~$ PWN=$(/challenge/run)
Congratulations! You have read the flag into the PWN variable. Now print it out
and submit it!
hacker@variables~storing-command-output:~$ echo $PWN
pwn.college{YWdnQlvfw1andSHi6tqZta0lcUT.QX1cDN1wSO1EzNzEzW}
```

## What I Learned
I learned how to store the output of a command directly to a variable

## References
None