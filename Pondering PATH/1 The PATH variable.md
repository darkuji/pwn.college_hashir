# The PATH variable
### The challenge asks us to set PATH to null so that rm is removed


## My Solve
**Flag:** pwn.college{g2uTeSArC4xo_YGopcduUlyHSmD.QX2cDM1wSO1EzNzEzW}
Used PATH="" so that the rm command is removed then ran /challenge/run
and obtained the flag as it couldn't delete it


```
hacker@path~the-path-variable:~$ PATH=""
hacker@path~the-path-variable:~$ /challenge/run
Trying to remove /flag...
/challenge/run: line 4: rm: No such file or directory
The flag is still there! I might as well give it to you!
pwn.college{g2uTeSArC4xo_YGopcduUlyHSmD.QX2cDM1wSO1EzNzEzW}
```

## What I Learned
Learned how PATH works and how clearing it can clear ls aswell

## References
None