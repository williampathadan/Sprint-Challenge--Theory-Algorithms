## Anwers - Algorithm

### Exercise I
    a. O(n)
    b. O(log n)
    c. O(sqrt(n))
    d. O(n log n)
    e. O(n^3)
    f. O(n)
    g. O(n)


### Exercise II

a)
```js
function getMaxDiff(array) {
  let min = array[0];
  let max = array[0];

  for (let i = 0; i < array.length; i++) {
    const value = array[i];

    if (value < min) min = value;
    if (value > max) max = value;
  }

  return max - min;
}
```

b) My strategy would be to use a Binary Search Tree like algorithm

    Let's start from floor `f = n/2`  
    If the egg breaks, then move down to `f = f/2`  
    Otherwise, move up to `f = f + (n - f)/2`  

    We will stop our search when egg doen't break at `f`,
    and egg breaks at `f + 1`.

    And, now we have value of f.


### Exercise III
a) Time complexity will be O(n^2) in this case. Because at every iteration the left array is empty while right array is of size (n-1), (n-2), ...

b) Time complexity in this case will be O(n log n). Because at every step the array is split into 2 almost equal sized arrays. Hence there will be (log n) number of steps, and each step has linear O(n) time complexity.