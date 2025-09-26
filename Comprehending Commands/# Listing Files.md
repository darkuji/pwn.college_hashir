# Listing Files
### The challenge asks us to list the files in a directory using the ls command


## My Solve
**Flag:** pwn.college{I0zP9iojfbHOfvlf2xffh72Rzx1.QX4IDO0wSO1EzNzEzW}
I first used the ls command with argument as /challenge to list the
elements of the directory then i used the absolute path of the renamed
run file in order to obtain the flag



```
hacker@commands~listing-files:~$ ls /challenge
5573-renamed-run-27418  DESCRIPTION.md
hacker@commands~listing-files:~$ /challenge/5573-renamed-run-27418
Yahaha, you found me! Here is your flag:
pwn.college{I0zP9iojfbHOfvlf2xffh72Rzx1.QX4IDO0wSO1EzNzEzW}
```

## What I Learned
I learned how the elements or files inside of a directory in a Linux
environment can be listed using the ls command by giving the absolute
path of the directory as an argument


## References
None