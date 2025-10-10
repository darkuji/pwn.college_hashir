# Scripting with arguments
### The challenge asks us to make a script which takes arguments


## My Solve
**Flag:** pwn.college{IBMgsQiNdEpY9Z5VYSfq6sWqgZp.0VNzMDOxwSO1EzNzEzW}
Used echo 'echo $2 $1' > /home/hacker/solve.sh to send it to the script 
the command is basically printing the two arguments in reverse order as 
$2 is the second one which is being printed first then used 
bash /home/hacker/solve.sh to run the script with arguments as
pwn and college then ran /challenge/run


```
hacker@chaining~scripting-with-arguments:~$ echo 'echo $2 $1' > /home/hacker/solve.sh
hacker@chaining~scripting-with-arguments:~$ bash /home/hacker/solve.sh pwn college
college pwn
hacker@chaining~scripting-with-arguments:~$ /challenge/run
Correct! Your script properly reversed the arguments.
Here's your flag:
pwn.college{IBMgsQiNdEpY9Z5VYSfq6sWqgZp.0VNzMDOxwSO1EzNzEzW}
```

## What I Learned
Learned how to make scripts that accept arguments

## References
None