# Your first shell script
### The challenge asks us to create our own shell scri-pt


## My Solve
**Flag:** pwn.college{ETF0zsUMvqj-oNnUWMpdl8TjCTC.QXxcDO0wSO1EzNzEzW}
Used echo /challenge/pwn > x.sh to move it to the shell named x.sh then
moved /challenge/college to it by running echo /challenge/college >> x.sh
then used bash to execute the script



```
hacker@chaining~your-first-shell-script:~$ echo /challenge/pwn > x.sh
hacker@chaining~your-first-shell-script:~$ echo /challenge/college >> x.sh
hacker@chaining~your-first-shell-script:~$ bash x.sh
Great job, you've written your first shell script! Here is the flag:
pwn.college{ETF0zsUMvqj-oNnUWMpdl8TjCTC.QXxcDO0wSO1EzNzEzW}
```

## What I Learned
I learned how to create a new script and move things to it and run it 
using bash

## References
None