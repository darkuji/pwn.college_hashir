# Explicit Relative Paths, From /
### The challenge asks us to use the explicit relative path of a file by using . to obtain the flag


## My Solve
**Flag:**pwn.college{8yw79QiQebHhDPilUWY6aMuG4EB.QXwUTN0wSO1EzNzEzW}
I first used the cd / command to change my working directory to '/' after which I used the 
'./' part along with the relative path of the file indicating that it is explicitly mentioned



```
hacker@paths~explicit-relative-paths-from-:~$ cd /
hacker@paths~explicit-relative-paths-from-:/$ ./challenge/run
Correct!!!
./challenge/run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{8yw79QiQebHhDPilUWY6aMuG4EB.QXwUTN0wSO1EzNzEzW}
```

## What I Learned
I learned how in a Linux environment the '.' entry can be used in a relative path file 
which is used to refer to files in the same directory

## References
None