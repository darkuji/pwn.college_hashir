# Grepping for a needle in a haystack
### The challenge asks us to use the grep command to search for a string in a text file


## My Solve
**Flag:** pwn.college{ovuoO2NBatXVwNQDWSpAWgSbJNt.QX3EDO0wSO1EzNzEzW}
I first used the grep command with 'pwn' as the search string as every flag
starts with the string pwn.college then i provided the absolute path of the
textfile in which the flag had to be searched and obtained the flag


```
hacker@commands~grepping-for-a-needle-in-a-haystack:~$ grep pwn /challenge/data.txt
pwning
pwn
pwn.college{ovuoO2NBatXVwNQDWSpAWgSbJNt.QX3EDO0wSO1EzNzEzW}
pwned
pwns
```

## What I Learned
I learned how we can search for a particular string in a textfile using the grep command 
by putting the string to be searched as the first argument and the absolute path of the file
to be searched from as the second argument


## References