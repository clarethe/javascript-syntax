<h1 align="center">
<br>
  <br>
    <br>
    Destructuring assignment
  <br><br>
</h1>
 

[![Visitor](https://visitor-badge.laobi.icu/badge?page_id=clarethe)](https://github.com/clarethe) [![GitHub followers](https://img.shields.io/github/followers/clarethe.svg?style=social&label=Follow)](https://github.com/clarethe?tab=followers)
 
The destructuring assignment syntax is a JavaScript expression that makes it possible to unpack values from arrays, or properties from objects, into distinct variables.

```
let a, b, rest;
[a, b] = [10, 20];

console.log(a);
// expected output: 10

console.log(b);
// expected output: 20

[a, b, ...rest] = [10, 20, 30, 40, 50, 60];

console.log(rest);
// expected output: Array [30,40,50]
```
+info [here](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)  