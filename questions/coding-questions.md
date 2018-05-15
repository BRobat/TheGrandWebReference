## Coding Questions:

#Question: What is the value of foo?

```javascript
var foo = 10 + '20';

```
answer:

foo equals '1020'


#Question: What will be the output of the code below?
```javascript
console.log(0.1 + 0.2 == 0.3);

```
answer:

should be true


#Question: How would you make this work?
```javascript
add(2, 5); // 7
add(2)(5); // 7
```
answer:

what do you mean? should I define the function?

```javascript
function add(a,b) {
    return a + b
}
```

```javascript


```

#Question: What value is returned from the following statement?
```javascript
"i'm a lasagna hog".split("").reverse().join("");

```
answer:

as join returns string to the state from before split. It's only reversed. 
So it's: "goh angasal a m'i"

#Question: What is the value of window.foo?
```javascript
( window.foo || ( window.foo = "bar" ) );

```
answer:



#Question: What is the outcome of the two alerts below?
```javascript
var foo = "Hello";
(function() {
  var bar = " World";
  alert(foo + bar);
})();
alert(foo + bar);

```
answer:

the alert will show: "Hello World"

#Question: What is the value of foo.length?
```javascript
var foo = [];
foo.push(1);
foo.push(2);

```
answer:

foo equals: [1, 2]

#Question: What is the value of foo.x?
```javascript
var foo = {n: 1};
var bar = foo;
foo.x = foo = {n: 2};

```
answer: 

foo.x is undefined 
foo is object Object

#Question: What does the following code print?
```javascript

console.log('one');
setTimeout(function() {
  console.log('two');
}, 0);
console.log('three');
```
answer:

for 0 seconds the answer is "onethree" but then it turns to "two"

#Question: What is the difference between these four promises?
```javascript
doSomething().then(function () {
  return doSomethingElse();
});

doSomething().then(function () {
  doSomethingElse();
});

doSomething().then(doSomethingElse());

doSomething().then(doSomethingElse);

```
answer:
