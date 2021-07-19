---
title: binary
tags: function,intermediate
firstSeen: 2020-05-13T13:36:36+03:00
lastUpdated: 2020-10-18T23:04:45+03:00
---

Creates a function that accepts up to two arguments, ignoring any additional arguments.

- Call the provided function, `fn`, with the first two arguments given.
- Note that the function provided to the Array.prototype.map() method can take 3 parameters. First one is the current element of the array. Second one is the index of that element (optional). The third parameter is the array itself (also optional).   

```js
const binary = fn => (a, b) => fn(a, b);
```

```js
['2', '1', '0'].map(binary(Math.max)); // [2, 1, 2]
```
