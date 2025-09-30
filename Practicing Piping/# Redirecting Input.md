# Redirecting Input
### The challenge asks us to redirect the input of a file to a program


## My Solve
**Flag:** pwn.college{E3eQrsDeS_EL4zKOhKsw9qIsr3T.QXwcTN0wSO1EzNzEzW}
I first had to store the value COLLEGE in the PWN file which i did using
the > command after which i used the < command to get the input in PWN as 
/challenge/run 


```
hacker@piping~redirecting-input:~$ echo COLLEGE > PWN
hacker@piping~redirecting-input:~$ cat PWN
COLLEGE
hacker@piping~redirecting-input:~$ /challenge/run < PWN
Reading from standard input...
Correct! You have redirected the PWN file into my standard input, and I read
the value 'COLLEGE' out of it!
Here is your flag:
pwn.college{E3eQrsDeS_EL4zKOhKsw9qIsr3T.QXwcTN0wSO1EzNzEzW}
```

## What I Learned
I learned how we can redirect input of files to other files using the < command

## References
None