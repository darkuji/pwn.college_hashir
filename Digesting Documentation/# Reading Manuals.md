# Reading Manuals
### The challenge asks us to use the man command to read the manual of a file


## My Solve
**Flag:** pwn.college{g3iUZOqYbgVu4OZNSD-O22m2cB9.QX0EDO0wSO1EzNzEzW}
I used the man challenge command to read the manual of the file where it 
said that /challenge/challenge has the flag and 3 arguments out of which the
-giqbgu was the useful one which is supposed to print the flag when we give
342 as an argument with it.


```
hacker@man~reading-manuals:~$ man challenge
hacker@man~reading-manuals:~$ /challenge/challenge --giqbgu 342
Correct usage! Your flag: pwn.college{g3iUZOqYbgVu4OZNSD-O22m2cB9.QX0EDO0wSO1EzNzEzW}

```

## What I Learned
I learned how we can add a manual for a file in a Linux environment which can
be used to give instructions to developers or users

## References
None