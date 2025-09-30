# Writing to multiple programs
### The challenge asks us to store the output and input in multiple programs


## My Solve
**Flag:** pwn.college{YoaVHGbITMl9fCoL8wZjHun2SX8.QXwgDN1wSO1EzNzEzW}
used /challenge/hack | tee >( /challenge/the ) | /challenge/planet
to store the output in both the and planet file


```
hacker@piping~writing-to-multiple-programs:~$ /challenge/hack | tee >( /challenge/the ) | /challenge/planet
Congratulations, you have duplicated data into the input of two programs! Here
is your flag:
pwn.college{YoaVHGbITMl9fCoL8wZjHun2SX8.QXwgDN1wSO1EzNzEzW}
```

## What I Learned
I learned how to store the output of a program in multiple files (duplicating)

## References
None