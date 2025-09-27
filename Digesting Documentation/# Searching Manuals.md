# Searching Manuals
### The challenge asks us to search inside a manual


## My Solve
**Flag:** pwn.college{gLOPZA5TW-TjrU1YWF3ndV1I3R5.QX1EDO0wSO1EzNzEzW}
I first read the manual of challenge and then used the / command to search
for the word flag , used n to go a few results further where i found that 
i need to use the --igy argument along with the /challenge/challenge program
to print the flag

```
hacker@man~searching-manuals:~$ man challenge
hacker@man~searching-manuals:~$ /challenge/challenge --igy
Initializing...
Correct usage! Your flag: pwn.college{gLOPZA5TW-TjrU1YWF3ndV1I3R5.QX1EDO0wSO1EzNzEzW}
```

## What I Learned
I learned how we can also search for keywords in a manual like we can use the find 
command in files to search for something if a manual is too big to manually search

## References
None