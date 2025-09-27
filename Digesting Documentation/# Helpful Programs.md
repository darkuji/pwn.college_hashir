# Helpful Programs
### The challenge asks us to use the --help argument with a program instead of man


## My Solve
**Flag:** pwn.college{o293oODvBbUnaMjnL_Y3bo46qvR.QX3IDO0wSO1EzNzEzW}
I used the --help argument with the program to find the instructions where 
it said i needed to use the -p argument to obtain a secret value which was 293
and i needed to use the -g command with the secret value to obtain the flag


```
hacker@man~helpful-programs:~$ /challenge/challenge --help
usage: a challenge to make you ask for help [-h] [--fortune] [-v] [-g GIVE_THE_FLAG] [-p]

optional arguments:
  -h, --help            show this help message and exit
  --fortune             read your fortune
  -v, --version         get the version number
  -g GIVE_THE_FLAG, --give-the-flag GIVE_THE_FLAG
                        get the flag, if given the correct value
  -p, --print-value     print the value that will cause the -g option to give you the flag
hacker@man~helpful-programs:~$ /challenge/challenge -p
The secret value is: 293
hacker@man~helpful-programs:~$ /challenge/challenge -g 293
Correct usage! Your flag: pwn.college{o293oODvBbUnaMjnL_Y3bo46qvR.QX3IDO0wSO1EzNzEzW}
```

## What I Learned
I learned how instead of man we can use the --help or -help argument with a program
which does more or less the same thing as man

## References
None