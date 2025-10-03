# Extracting the first lines with head
### The challenge asks us to extract the first few lines of a program 


## My Solve
**Flag:** pwn.college{kriLKLmsM5CbS66-xql9yhf7SCN.0lNxEzNxwSO1EzNzEzW}
used head -n 7 so that the first 7 lines of the program are read then
piped it directly to /challenge/college since it had secret codes which 
were of no use to me


```
hacker@data~extracting-the-first-lines-with-head:~$ /challenge/pwn | head -n 7 | /challenge/college
Congratulations, you piped the right codes!
pwn.college{kriLKLmsM5CbS66-xql9yhf7SCN.0lNxEzNxwSO1EzNzEzW}
```

## What I Learned
I learned how we can display a certain number of lines from the start
of a program in a Linux environment using the head command 

## References
None