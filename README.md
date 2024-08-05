# Recursions

## Sample problem at hand
Add all non-negative integers upto n.

### solutions:
1. Using loops

Here is how this can be solved with the use of a for loop.

``` python
def sum(n):
    sum = 0
    for i in range(n + 1):
        sum += i
    return sum

print(sum(10))# Returns 55
```

In JavaScript:

``` js
function sum(n) {
    let sum = 0;
    for (let i = 0; i <= n; i++) {
        sum += 1;
    }
    return sum;
}

console.log(10) // returns 55
```