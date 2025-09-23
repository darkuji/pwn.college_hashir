# Removing Files
### The challenge asks us to remove files


## My Solve
**Flag:** pwn.college{A-mpVWyeGVYBNOVWTUrqHLoMoV0.QX2kDM1wSO1EzNzEzW}
I first used the ls command to list the files in the directory to 
see the name of the file to be deleted. Then I used the rm command
along with the name of the file to delete it and obtained the flag



```
hacker@commands~removing-files:~$ ls
a  delete_me
hacker@commands~removing-files:~$ rm delete_me
hacker@commands~removing-files:~$ /challenge/check
Excellent removal. Here is your reward:
pwn.college{A-mpVWyeGVYBNOVWTUrqHLoMoV0.QX2kDM1wSO1EzNzEzW}
```

## What I Learned
I learned how we can also remove files from a Linux environment
by using the rm command and passing the file name as as argument

## References
None