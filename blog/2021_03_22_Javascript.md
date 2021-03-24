# Basic Javascript

## Conditional Statement

### True/Flase Check

The expression considered as **false**:
- flase
- 0
- Empty String
- NaN
- undefined
- null

The expression considered as **true**:
- ture
- Any number other than 0
- Non-empty string
- Non-empty object
---
### === and ==
== checks value hence, === checks both value and data type

- "5"==5 // return true
- "5"===5 // return false
---
### Object Comparsion
Although the objects are equivalent, the comparsion return false becuase these objects have different addresses in memory

var obj1 = {};
var obj2 = {};

- obj1==obj2 // return false
- obj1===obj2 // return false

## String

In javascript, String object has many useful built-in functions.

### Regex

Here is the Regex Rule:
- ^ : indicates the start of a string/line
- \d : finds any digits
- \[abc\] : finds any char between the brackets
- \[^abc\] : finds any char not between the brackets
- \[0-9\] : finds any digit between the brackets
- \[^0-9\] : finds any digit not between the brackets
- (x|y) : finds any of the alternatives specified

### Encoding

Javascript has built-in encoding and decoding function, BtoA, AtoB

btoa() - creates a base64-encoded ASCII strings from a string
atob() - decodes a string of data that has been encoded using base64 encoding

## For Loop

Beside the traditional for loop format for (Variables; Condition; Modification),

### for (in)
Before in, the variable specified as index
```javascript
var array = [1, 2, 3]
for (var index in array) {
    console.log(index) // retruns 0, 1, 2
}

for (var index in array) {
    console.log(array[index]) // retruns 1, 2, 3
}
```

### for (of)
Before of, the variable specified as element
```javascript
for (var element of array) {
    console.log(element) // returns 1, 2, 3
}
```

