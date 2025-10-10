# Scripting with default case
### The challenge asks us to make a script with default case


## My Solve
**Flag:** pwn.college{UdrlpSu9IJ4vW1hv8TBdiVWBaKJ.01NzMDOxwSO1EzNzEzW}
Everything same as last challenge but added an else block which prints nope
whenever the input isn't pwn


```
hacker@chaining~scripting-with-default-cases:~$ echo '#!/bin/sh' > /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo 'case "$1" in' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '  pwn)' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '    echo "college"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '    ;;' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '  *)' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '    echo "nope"' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo '    ;;' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ echo 'esac' >> /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ chmod +x /home/hacker/solve.sh
hacker@chaining~scripting-with-default-cases:~$ /challenge/run
Correct! Your script properly handles the if/else conditions.
Here's your flag:
pwn.college{UdrlpSu9IJ4vW1hv8TBdiVWBaKJ.01NzMDOxwSO1EzNzEzW}
```

## What I Learned
Learned how to make a script with a default case

## References
ChatGPT