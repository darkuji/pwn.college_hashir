# Setting PATH
### The challenge asks us to set PATH to a directory


## My Solve
**Flag:** pwn.college{0JlzxEUBptgToz1dCRS-gA7suEi.QX1cjM1wSO1EzNzEzW}
used PATH=/challenge/more_commands/ coz we needed the win command which
was stored in this directory then ran /challenge/run to obtain the flag


```
hacker@path~setting-path:~$ PATH=/challenge/more_commands/
hacker@path~setting-path:~$ /challenge/run
Invoking 'win'....
Congratulations! You properly set the flag and 'win' has launched!
pwn.college{0JlzxEUBptgToz1dCRS-gA7suEi.QX1cjM1wSO1EzNzEzW}
```

## What I Learned
Learned how to set PATH to a directory 

## References
None