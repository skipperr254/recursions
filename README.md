# Recursions

## Sample problem at hand
Add all non-negative integers upto n.

### solutions:
1. Using loops

Here is how this can be solved with the use of a for loop.

``` python
# Python
def sum(n):
    sum = 0
    for i in range(n + 1):
        sum += i
    return sum

print(sum(10))# Returns 55
```

In JavaScript:

``` js
// JS
function sum(n) {
    let sum = 0;
    for (let i = 0; i <= n; i++) {
        sum += 1;
    }
    return sum;
}

console.log(10) // returns 55
```
2. Adding Mathematically

Python solution:
``` python
# Python
def sum(n):
    return int(n * (n + 1) / 2)

print(sum(10))
```

JavaScritp solution:
``` js
// JS
function sum(n) {
    return n * (n + 1) / 2;
}

console.log(sum(10));
```