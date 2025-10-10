# Scripting With Conditions
### The challenge asks us to create a script that works with conditions


## My Solve
**Flag:** pwn.college{Ihi9mEwW-yVkvBlbya7opcMsAl7.0lNzMDOxwSO1EzNzEzW}
Used echo 'if [ "$1" == "pwn" ]' > /home/hacker/solve.sh which checkds 
if the first argument is pwn then used  echo 'then' >> /home/hacker/solve.sh
and  echo ' echo "college"' >> /home/hacker/solve.sh to print college if the condition
is true then used echo 'fi' >> /home/hacker/solve.sh to close the if block then 
ran /challenge/run


```
hacker@chaining~scripting-with-conditionals:~$ echo 'if [ "$1" == "pwn" ]' > /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ echo 'then' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ echo ' echo "college"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ bash /home/hacker/solve.sh pwn
/home/hacker/solve.sh: line 4: syntax error: unexpected end of file
hacker@chaining~scripting-with-conditionals:~$ bash /home/hacker/solve.sh pwn
/home/hacker/solve.sh: line 4: syntax error: unexpected end of file
hacker@chaining~scripting-with-conditionals:~$ echo 'fi' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-conditionals:~$ bash /home/hacker/solve.sh pwn
college
hacker@chaining~scripting-with-conditionals:~$ /challenge/run
Correct! Your script properly handles all the conditions.
Here's your flag:
pwn.college{Ihi9mEwW-yVkvBlbya7opcMsAl7.0lNzMDOxwSO1EzNzEzW}
```

## What I Learned
Learned how to create scripts with conditionals

## References
None