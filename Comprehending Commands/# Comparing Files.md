# Comparing Files
### The challenge asks us to use the diff command with two files as arguments to compare them


## My Solve
**Flag:** pwn.college{MpVN5cCOEYlU2HA94ovyG_aVLfn.01MwMDOxwSO1EzNzEzW}
I first used the diff command with the first argument as the file with decoy
flags and the file with the extra real flag then the output was 4a5 along 
with the flag indicating that after line 4 of file 1 add line 5 of file 2



```
hacker@commands~comparing-files:~$ diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt
4a5
> pwn.college{MpVN5cCOEYlU2HA94ovyG_aVLfn.01MwMDOxwSO1EzNzEzW}
```

## What I Learned
I learned how instead of manually scanning a file in a Linux environment
we can just use the diff command and enter the paths or names of the files
to compare the differences between them

## References
None