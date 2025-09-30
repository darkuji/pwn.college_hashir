# Process Substitution for Input
### The challenge asks us to differentiate between outputs directly


## My Solve
**Flag:** pwn.college{sJH3ZLAMC1auDFRIxpyngWqvrdj.0lNwMDOxwSO1EzNzEzW}
I used the command diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
to directly get the difference between the outputs of the two files


```
hacker@piping~process-substitution-for-input:~$ diff <(/challenge/print_decoys) <(/challenge/print_decoys_and_flag)
48a49
> pwn.college{sJH3ZLAMC1auDFRIxpyngWqvrdj.0lNwMDOxwSO1EzNzEzW}
```

## What I Learned
Outputs of programs can be differentiated directly without having to store the output
in separate files

## References
None