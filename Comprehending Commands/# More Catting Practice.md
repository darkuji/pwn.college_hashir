# More Catting Practice
### The command asks us to use the absolute path as an argument with the cat command


## My Solve
**Flag:** pwn.college{UGNI0ZMzU2yyQOyJbormL6S8j11.QXwITO0wSO1EzNzEzW}
I first used the cat command and then passed the argument /usr/share/lintian/flag 
which is the absolute path of the file where the flag is stored


```
hacker@commands~more-catting-practice:~$ cat /usr/share/lintian/flag
pwn.college{UGNI0ZMzU2yyQOyJbormL6S8j11.QXwITO0wSO1EzNzEzW}
```

## What I Learned
I learned how in a Linux environment we can use the absolute path of a file
as an argument in the cat command

## References
None