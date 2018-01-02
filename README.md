# Functional-programming. 


## Topics in functional programming mainly in javascript such as:


1- Pure functions vs Impure functions.
  
  Impure functions are functions the change the state of a program. Since they change the the state of the program, they are called "functions with side effects" becasue they got access to things outside their scope and modify them. Pure functions elimates this problem by wraping an impure function around a pure function "clousre". This is an example. 
  
  
```javascript

function foo(x) {
    y++; 
    z = x * y ; 
}

var y = 5 ,  z ; 
foo(5);
console.log(z); 
```

This example of javascript code changes the state of some variables in the global scope by calling the function foo().  This is an example of a impure function. 


However, to make this example pure, we need to wrap the impure function foo around a pure function, and let's call it bar.


```javascript
function bar(x, y) {
    let z ; 
    foo(x);
    return z ; 
function foo(x) {
    y++; 
    z = x * y ; 
}
}
console.log(bar(5,6));
```


2- Composition.

3- Immutability.

4- Closures.Very important in programming languages in general.

5- Recursion. sed in other programming paradigms, but it is heavily related to functional programming.

6- List-transformation (map).

7- List-exclusion (filter).

8- List-composition (reduce).

9- List-iteration.



