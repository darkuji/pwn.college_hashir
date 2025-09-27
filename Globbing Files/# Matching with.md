# Matching with *
### The challenge asks us to use the * command to search for files


## My Solve
**Flag:** pwn.college{ckpJAJDGAaTZ1Nifht8S8SGCZEi.QXxIDO0wSO1EzNzEzW}
I used the cd /ch* command to change cwd to challenge as only 4
characters could be passed then i used /challenge/run to obtain 
the flag

```
hacker@globbing~matching-with-:~$ cd /ch*
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{ckpJAJDGAaTZ1Nifht8S8SGCZEi.QXxIDO0wSO1EzNzEzW}
```

## What I Learned
I learned how instead of typing entire names we can use * to search
for files or to search for files which have a similar prefix

## References
None