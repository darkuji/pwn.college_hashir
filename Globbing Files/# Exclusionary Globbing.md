# Exclusionary Globbing
### The challenge asks us to exclude files that are named a certain way


## My Solve
**Flag:** pwn.college{I8jSakYiM1f3_rNAz3RWYgQ7Tdr.QX2IDO0wSO1EzNzEzW}
I used the [!pwn] part to exclude the files that have pwn in them and the *
after it indicating that i only wanna exlude files that start with p w or n

```
hacker@globbing~exclusionary-globbing:~$ cd /challenge/files
hacker@globbing~exclusionary-globbing:/challenge/files$ /challenge/run [!pwn]*
You got it! Here is your flag!
pwn.college{I8jSakYiM1f3_rNAz3RWYgQ7Tdr.QX2IDO0wSO1EzNzEzW}
```

## What I Learned
I learned how like searching for a particular character we can also
choose to exclude a particular character (or multiple) using globbing

## References
None