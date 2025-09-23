# Implicit Relative Paths, From /
### The challenge asks us to use the relative path of a program instead of its absolute path


## My Solve
**Flag:** pwn.college{A8g6WUksVGM6qsbPcFn2bhso93e.QX5QTN0wSO1EzNzEzW}
I first used the 'cd' command to change my working directory to /, then i used the challenge/run
statement to get the flag as that is the relative path of the file in the directory '/'



```
hacker@paths~implicit-relative-paths-from-:/$ cd /
hacker@paths~implicit-relative-paths-from-:/$ challenge/run
Correct!!!
challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{A8g6WUksVGM6qsbPcFn2bhso93e.QX5QTN0wSO1EzNzEzW}
```

## What I Learned
I learned the difference between the relative and absolute path of a file in a Linux
environment. Further i learned how to use the relative path of a file to save time by 
not having to refer to its entire location repeatedly 


## References

None
