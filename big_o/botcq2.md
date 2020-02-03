# Quiz 2

1. What is the time complexity for the following function

   1. O(n)

```
  function logUpTo(n) {
      for (var i = 1; i <= n; i++) {
        console.log(i)
      }
    }
```

2. What is the time complexity for the following function

   2. O(1)
      <!-- This function will only log up to 10, if n is bigger than 10, therefore it stays constant -->

```
  function logAtMost10(n) {
    for (var i = 1; i <= Math.min(n, 10); i++) {
      console.log(i)
    }
  }
```

3. What is the time complexity for the following function

   3. O(n)
      <!-- This function will log up to 10, for inputs smaller or equal to 10, anything higher will be linear time  -->

```
  function logAtLeast(n) {
    for(var i = 1; i <= Math.max(n, 10); i++) {
      console.log(i)
    }
  }
```

4. What is the time complexity for the following function

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

5. What is the time complexity for the following function

   5. O(n^2)

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
