Today I learned a straight-forward way to swap the values of two variables in JavaScript.

Say `var a = 10` and `var b = 20`.

Previously, I would use the following (tedious) strategy to swap the values:
``` javascript
var temp = a;  // temp is now 10
a = b;         // a is now 20
b = temp;      // b is now 10
```

An quicker way to do this is:
``` javascript
b = [a, a = b][0];
```

Or even, in ECMAScript 6:
``` javascript
[a, b] = [b, a];
```
