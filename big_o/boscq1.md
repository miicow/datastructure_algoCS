# Quiz 1

1. What is the space complexity for the following function

   1. O(1)

```
  function logUpTo(n) {
      for (var i = 1; i <= n; i++) {
        console.log(i)
      }
    }
```

2. What is the space complexity for the following function

   2. O(1)

```
  function logAtLeast(n) {
    for(var i = 1; i <= Math.max(n, 10); i++) {
      console.log(i)
    }
  }
```

3. What is the space complexity for the following function

   3. O(1)

```
  function logAtMost10(n) {
    for (var i = 1; i <= Math.min(n, 10); i++) {
      console.log(i)
    }
  }
```

4. What is the space complexity for the following function

   4. O(n)

```
  function onlyElementsAtEvenIndex(array) {
    var newArray = Array(Math.ceil(array.length / 2));
    for (var i = 0; i < array.length; i++) {
      if (i % 2 === 0) {
        newArray[i / 2] = array[i];
      }
    }
    return newArray;
  }
```

5. What is the space complexity for the following function

   5. O(n)

```
  function subtotals(array) {
    var subtotalArray = Array(array.length);
    for(var i = 0; i < array.length; i++) {
      var subtotal = 0;
      for(var j = 0; j <= i; j++) {
        subtotal += array[j];
      }
      subtotalArray[i] = subtotal;
    }
    return subtotalArray;
  }
```
