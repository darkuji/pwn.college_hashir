# Moving Files
### The challenge asks us to move a file to another directory using the mv command


## My Solve
**Flag:** pwn.college{Q6b9pWQhpDKnNgxRayjnNPXZaCl.0VOxEzNxwSO1EzNzEzW}
I first used the mv command with the first argument as the file to be 
moved and 2nd argument as the file to be moved to



```
hacker@commands~moving-files:~$ mv /flag /tmp/hack-the-planet
Correct! Performing 'mv /flag /tmp/hack-the-planet'.
hacker@commands~moving-files:~$ /challenge/check
Congrats! You successfully moved the flag to /tmp/hack-the-planet! Here it is:
pwn.college{Q6b9pWQhpDKnNgxRayjnNPXZaCl.0VOxEzNxwSO1EzNzEzW}
```

## What I Learned
I learned how in a Linux environment we can use the mv command to move files
from one place to another by passing them as arguments 

## References
None