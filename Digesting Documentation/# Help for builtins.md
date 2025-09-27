# Help for builtins
### The challenge asks us to use the help command for a specific file to get instructions


## My Solve
**Flag:** pwn.college{wxj_p_IcagVyHAJFkmJloEZ6Aoc.QX0ETO0wSO1EzNzEzW}
I used the help challenge command to get to know the instructions where
i found out that i need to use the --secret argument with a value which 
was already given. I used the --secret command with the value to get the 
flag

```
hacker@man~help-for-builtins:~$ help challenge
challenge: challenge [--fortune] [--version] [--secret SECRET]
    This builtin command will read you the flag, given the right arguments!

    Options:
      --fortune         display a fortune
      --version         display the version
      --secret VALUE    prints the flag, if VALUE is correct

    You must be sure to provide the right value to --secret. That value
    is "wxj_p_Ic".
hacker@man~help-for-builtins:~$ challenge --secret wxj_p_Ic
Correct! Here is your flag!
pwn.college{wxj_p_IcagVyHAJFkmJloEZ6Aoc.QX0ETO0wSO1EzNzEzW}
```

## What I Learned
I learned how we can use help command for a specific file aswell in a Linux
environment 

## References
None