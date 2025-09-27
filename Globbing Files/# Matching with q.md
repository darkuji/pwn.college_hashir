# Matching with ?
### The challenge asks to search using ? command


## My Solve
**Flag:** pwn.college{4XcKBzCKpY0aKnVDHyvjkE2ryYj.QXyIDO0wSO1EzNzEzW}
I used the cd /?ha??enge command as ? replaces any character but it 
changed cwd to challenge as that was the only directory matching the other
conditions after which i used /challenge/run to get the flag


```
hacker@globbing~matching-with-:~$ cd /?ha??enge
hacker@globbing~matching-with-:/challenge$ /challenge/run
You ran me with the working directory of /challenge! Here is your flag:
pwn.college{4XcKBzCKpY0aKnVDHyvjkE2ryYj.QXyIDO0wSO1EzNzEzW}
```

## What I Learned
I learned how while searching for files we can use ? as a character if 
we are flexible with it or are unsure

## References
None