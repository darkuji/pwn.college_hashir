# Redirecting Script output
### The challenge asks us to redirect script output


## My Solve
**Flag:** pwn.college{wsx3O1f66VoPU58RWg_VV0SMfoy.QX4ETO0wSO1EzNzEzW}
Used echo /challenge/pwn > x.sh to send that data to the shell named x
then used echo /challenge/colleg >> x.sh to send that aswell then used 
bash x.sh with | /challenge/solve to pipe the output of the script to 
/challenge/solve


```
hacker@chaining~redirecting-script-output:~$ echo /challenge/pwn > x.sh
hacker@chaining~redirecting-script-output:~$ echo /challenge/college >> x.sh
hacker@chaining~redirecting-script-output:~$ bash x.sh | /challenge/solve
Correct! Here is your flag:
pwn.college{wsx3O1f66VoPU58RWg_VV0SMfoy.QX4ETO0wSO1EzNzEzW}
```

## What I Learned
I learned how to redirect the output of a script

## References
None