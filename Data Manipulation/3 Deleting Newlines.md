# Deleting Newlines
### The challenge asks us to delete new lines from the output


## My Solve
**Flag:** pwn.college{gYx_1ra_JtdDULgmhwfBqdeNlJ6.0VNxEzNxwSO1EzNzEzW}
used tr -d "\n" to not display any line breaks in the output


```
hacker@data~deleting-newlines:~$ /challenge/run | tr -d "\n"
Your line-split flag: pwn.college{gYx_1ra_JtdDULgmhwfBqdeNlJ6.0VNxEzNxwSO1EzNzEzW}
```

## What I Learned
I learned how we can separate linebreaks from the output while printig

## References
None