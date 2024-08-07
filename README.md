# Recursions

## Sample problem at hand
Problem 1: Add all non-negative integers upto n.

### Solutions:
#### 1. Using loops

Here is how this can be solved with the use of a for loop. This involves using a for loop to loop over all integers upto n and add them one by one.

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
#### 2. Adding Mathematically  
This involves using the mathematical formula:
`Sn = n(n+1)/2`  
where Sn is the sum of all of the first n integers.

Python solution:
``` python
# Python
def sum(n):
    return int(n * (n + 1) / 2)

print(sum(10))
```

JavaScript solution:
``` js
// JS
function sum(n) {
    return n * (n + 1) / 2;
}

console.log(sum(10));
```

#### 3. Recursion

With this method, a function that calls itself calls itself until a base case is achieved exiting the recursion.  

To create a recurive solution:  
1. Find the simplest possible input to the function.
    For example, in this integer addition problem, the simplest case scenario would be an input of 0 which gives an output of 0.

    ```python
    sum(0) --> 0
    ```
    In this example, giving an input of 0 should give an output of 0 as the sum of all integers upto 0 is, you guessed it, 0.
    This often translates to our base case for the recursion.





# Closing remarks - I leave you one piece of advice
**The Recursive leap of faith!** --> Assume simpler cases work out!