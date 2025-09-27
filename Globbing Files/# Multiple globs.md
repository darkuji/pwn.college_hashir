# Multiple globs
### The challenge asks us to use two globs at a time


## My Solve
**Flag:** pwn.college{kdxETqISXakTMfQ4Nu_LDBqTWZm.0lM3kjNxwSO1EzNzEzW}
I first changed my cwd to /challenge/files and as asked in the problem
i used the double glob with p (*p*) with the /challenge/run command 
to get the flag

```
hacker@globbing~multiple-globs:~$ cd /challenge/files
hacker@globbing~multiple-globs:/challenge/files$ /challenge/run *p*
You got it! Here is your flag!
pwn.college{kdxETqISXakTMfQ4Nu_LDBqTWZm.0lM3kjNxwSO1EzNzEzW}
```

## What I Learned
I learned how a file can be globbed from both sides like if we
know the middle characters of  file we can use *c* where c is the
letter 

## References
None