# Executable shell scripts
### The challenge asks us to make an executable shell script


## My Solve
**Flag:** pwn.college{EN9XfgvhGHlXnn-J8YogrrqjJWI.QX0cjM1wSO1EzNzEzW}
Used echo /challenge/solve > script.sh to send it to the script then 
used chmod a+x so that i can executable by everyone then executed it using
./


```
hacker@chaining~executable-shell-scripts:~$ echo /challenge/solve > script.sh
hacker@chaining~executable-shell-scripts:~$ chmod a+x script.sh
hacker@chaining~executable-shell-scripts:~$ ./script.sh
Congratulations on your shell script execution! Your flag:
pwn.college{EN9XfgvhGHlXnn-J8YogrrqjJWI.QX0cjM1wSO1EzNzEzW}
```

## What I Learned
I learned how we can make executable shell scripts and run them using ./ 
instead of bash

## References
None