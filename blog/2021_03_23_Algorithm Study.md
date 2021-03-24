# Algorithm Study

I've started solving algorithm problems at [leetcode](https://leetcode.com)

Try with the Two Sum, which is the easiest problem in the website.

Let me know if you want some assistance ;)

## Definition

> In mathematics and computer science, an algorithm is a finite sequence of well-defined, computer-implementable instructions, typically to solve a class of problems or to perform a computation. Algorithms are always unambiguous and are used as specifications for performing calculations, data processing, automated reasoning, and other tasks.

## How to study

Studying algorithm is nightmare.
Personally, I picked my comfortable language which is javacsript.
Luckily, I found the algorithm textbook called "JavaScript Data Structures and Algorithms - An Introduction to Understanding and Implementing Core Data Structure and Algorithm Fundamentals by Sammie Bae".

**Good Luck y'all**


## Sample Code
---
**BIG O NOTATION**

*O(n)*
```javascript
function Linear(n) {
    for(var i=0; i<n; i++) {
        console.log(i)
    }
}
```

*O(n^2)*
```javascript
function Quadratic(n) {
    for(var i=0; i<n; i++) {
        console.log(i)
        for(var j=0; j<n; j++) {
            console.log(j)
        }
    }
}
```

*O(n^3)*
```javascript
function Cubic(n) {
    for(var i=0; i<n; i++) {
        console.log(i)
        for(var j=i; j<n; j++) {
            console.log(j)
            for(var k=j; j<n; j++) {
                console.log(k)
            }
        }
    }
}
```

