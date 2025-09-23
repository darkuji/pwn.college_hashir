# Implicit Relative Path
### The challenge asks us to change the working directory and use '.' to mention relative file path


## My Solve
**Flag:**pwn.college{oGichVd-zhUCH4udIAHUFZiEd-0.QXxUTN0wSO1EzNzEzW}
I first changed the current working directory to /challenge using the cd command
and then I used the './' operator before mentioning the relative path of the 
file 'run' as Linux does not accept 'naked' paths in the cwd


```
hacker@paths~implicit-relative-path:/challenge$ cd /challenge
hacker@paths~implicit-relative-path:/challenge$ ./run
Correct!!!
./run is a relative path, invoked from the right directory!
Here is your flag:
pwn.college{oGichVd-zhUCH4udIAHUFZiEd-0.QXxUTN0wSO1EzNzEzW}
```

## What I Learned
I learned how in order to refer to the relative path of a file in the working
directory we must use the './' prefix as it avoids the execution of files in 
the cwd that have the same name as that of files in the core system utilities

## References
None