# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

The mystery function in the previous piece of code recursively searches an array for the maximum element. 
It compares the 1st element against the recursive call of the function with the remainder of the array.
That recursive call searches the remaining array and returns the largest element found. When there is
only one element left in the array it returns that element.
