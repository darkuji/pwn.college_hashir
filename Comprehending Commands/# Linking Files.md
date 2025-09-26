# Linking Files
### The challenge asks us to create a symbolic link between two files


## My Solve
**Flag:** pwn.college{0MUh0azu7Qx7ghbiZa4uVnctA2E.QX5ETN1wSO1EzNzEzW}
I first created a link between the original flag and the not the flag file
so that when i execute the /challenge/catflag command it opens the not the
flag command which contains the original flag because of the link


```
hacker@commands~linking-files:~$ ln -s /flag ~/not-the-flag
hacker@commands~linking-files:~$ /challenge/catflag
About to read out the /home/hacker/not-the-flag file!
pwn.college{0MUh0azu7Qx7ghbiZa4uVnctA2E.QX5ETN1wSO1EzNzEzW}
```

## What I Learned
I learned how we can create a link between two files which is like a 
shallow copy of a variable in some programming languages

## References
None