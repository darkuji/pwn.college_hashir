# Deleting characters
### The challenge asks us to delete characters in the output of a prorgram


## My Solve
**Flag:** pwn.college{Adnp1geUVlap9TN9dDQsQFn5B-Z.0FNxEzNxwSO1EzNzEzW}
Used tr -d ^% so that the output doesn't contain any ^ or %


```
hacker@data~deleting-characters:~$ /challenge/run | tr -d ^%
Your character-stuffed flag:
pwn.college{Adnp1geUVlap9TN9dDQsQFn5B-Z.0FNxEzNxwSO1EzNzEzW}
```

## What I Learned
I learned how we can filter the output for certain characters using
the tr -d command

## References
None