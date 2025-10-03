# Translating Characters
### The challenge asks us to translate characters by replacing them


## My Solve
**Flag:** pwn.college{U5rI5q5JQpVWvCUL93_NC2DM9pg.01MxEzNxwSO1EzNzEzW}
Used /challenge/run with tr so that it replaces all the small characters
with capital characters and vice versa


```
hacker@data~translating-characters:~$ /challenge/run | tr ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
yOUR CASE-SWAPPED FLAG:
pwn.college{U5rI5q5JQpVWvCUL93_NC2DM9pg.01MxEzNxwSO1EzNzEzW}
```

## What I Learned
Learned how we can replace certain characters in the output of a program
with desired characters

## References
None