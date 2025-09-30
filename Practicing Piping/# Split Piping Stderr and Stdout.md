# Split Piping Stderr and Stdout
### The challenge asks us to direct the std error and std output of a program to diff files


## My Solve
**Flag:** pwn.college{wSjeUWekMZWy9Y1ixsGuNL8KeJ_.QXxQDM2wSO1EzNzEzW}


```
hacker@piping~split-piping-stderr-and-stdout:~$ /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the )
Congratulations, you have learned a redirection technique that even experts
struggle with! Here is your flag:
pwn.college{wSjeUWekMZWy9Y1ixsGuNL8KeJ_.QXxQDM2wSO1EzNzEzW}
```

## What I Learned
Used prior knowledge

## References
None