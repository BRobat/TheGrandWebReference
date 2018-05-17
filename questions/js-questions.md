
### 1. Explain event delegation  
answer:  
Event delegation allows us to attach a single event listener (for example cell in a table) to a parent element (table), that will fire for all descendants matching a selector, whether those descendants exist now or are added in the future.

### 2. Explain how event delegation works in JavaScript  
answer:  
The best explanation I think is thru code. So here is some code for highlighting cells in a table:

```html
<table>
  <tr>
    <th colspan="3"><em>Bagua</em> Chart: Direction, Element, Color, Meaning</th>
  </tr>
  <tr>
    <td>...<strong>Northwest</strong>...</td>
    <td>...</td>
    <td>...</td>
  </tr>
  <tr>...2 more lines of this kind...</tr>
  <tr>...2 more lines of this kind...</tr>
</table>
```

```javascript
table.onclick = function(event) {
    let td = event.target.closest('td');

    if (!td) return;

    if (!table.contains(td)) return;

    highlight(td);
};
```
...method `elem.closest(selector)` returns the nearest ancestor that matches the selector. In our case we look for `<td>` on the way up from the source element.
...If `event.target` is not inside any `<td>` then the call returns null, and we don't have to do anything.
...In case of nested tables, `event.target` may be a `<td>` lying outside of the current table. So we check of that's actually our table's `<td>`
...And, if it's so, then higlight it.


### 3. Explain how prototypal inheritance works  
answer:  
What is prototype?  
A prototype of an object is just another object that is used as fallback source of properties. When an object gets a request for a property that it does not have, its prototype will be searched for the property, then the prototype’s prototype, and so on.  
What is inheritance?  


Now as we know what inheritance and prototype are

### 4. What do you think of AMD vs CommonJS?  
answer:

### 5. Explain why the following doesn't work as an IIFE: `function foo(){ }();`.  
answer:

### 6. What needs to be changed to properly make it an IIFE?  
answer:

### 7. What's the difference between a variable that is: null, undefined or undeclared?  
answer:

### 8. How would you go about checking for any of these states?  
answer:

### 9. What is a closure, and how/why would you use one?  
answer:

### 10. Can you describe the main difference between a forEach loop and a .map() loop and why you would pick one versus the other?  
answer:

### 11. What's a typical use case for anonymous functions?  
answer:

### 12. How do you organize your code? (module pattern, classical inheritance?)  
answer:

### 13. What's the difference between host objects and native objects?  
answer:

### 14. Difference between: function Person(){}, var person = Person(), and var person = new Person()?  
answer:

### 15. What's the difference between .call and .apply?  
answer:

### 16. Explain Function.prototype.bind.  
answer:

### 17. What's the difference between feature detection, feature inference, and using the UA string?  
answer:

### 18. Explain Ajax in as much detail as possible.  
answer:

### 19. What are the advantages and disadvantages of using Ajax?  
answer:

### 20. Explain how JSONP works (and how it's not really Ajax).  
answer:

### 21. Have you ever used JavaScript templating?  
answer:

### 22. If so, what libraries have you used?  
answer:

### 23. Explain "hoisting".  
answer:

### 24. Describe event bubbling.  
answer:

### 25. What's the difference between an "attribute" and a "property"?  
answer:

### 26. Why is extending built-in JavaScript objects not a good idea?  
answer:

### 27. Difference between document load event and document DOMContentLoaded event?  
answer:

### 28. What is the difference between == and ===?  
answer:

### 29. Explain the same-origin policy with regards to JavaScript.  
answer:

### 30. Make this work: duplicate([1,2,3,4,5]); // [1,2,3,4,5,1,2,3,4,5]  
answer:

### 31. Why is it called a Ternary operator, what does the word "Ternary" indicate?  
answer:

### 32. What is "use strict";? what are the advantages and disadvantages to using it?  
answer:

### 33. Create a for loop that iterates up to 100 while outputting "fizz" at multiples of 3, "buzz" at multiples of 5 and "fizzbuzz" at multiples of 3 and 5  
answer:

### 34. Why is it, in general, a good idea to leave the global scope of a website as-is and never touch it?  
answer:

### 35. Why would you use something like the load event? Does this event have disadvantages? Do you know any alternatives, and why would you use those?  
answer:

### 36. Explain what a single page app is and how to make one SEO-friendly.  
answer:

### 37. What is the extent of your experience with Promises and/or their polyfills?  
answer:

### 38. What are the pros and cons of using Promises instead of callbacks?  
answer:

### 39. What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?  
answer:

### 40. What tools and techniques do you use debugging JavaScript code?  
answer:

### 41. What language constructions do you use for iterating over object properties and array items?  
answer:

### 42. Explain the difference between mutable and immutable objects.  
answer:

### 43. What is an example of an immutable object in JavaScript?  
answer:

### 44. What are the pros and cons of immutability?  
answer:

### 45. How can you achieve immutability in your own code?  
answer:

### 46. Explain the difference between synchronous and asynchronous functions.  
answer:

### 47. What is event loop?  
answer:

### 48. What is the difference between call stack and task queue?  
answer:

### 49. Explain the differences on the usage of foo between function foo() {} and var foo = function() {}  
answer:

### 50. What are the differences between variables created using let, var or const?  
answer:

### 51. What are the differences between ES6 class and ES5 function constructors?  
answer:

### 52. Can you offer a use case for the new arrow => function syntax? How does this new syntax differ from other functions?  
answer:

### 53. What advantage is there for using the arrow syntax for a method in a constructor?  
answer:

### 54. What is the definition of a higher-order function?  
answer:

### 55. Can you give an example for destructuring an object or an array?  
answer:

### 56. ES6 Template Literals offer a lot of flexibility in generating strings, can you give an example?  
answer:

### 57. Can you give an example of a curry function and why this syntax offers an advantage?  
answer:

### 58. What are the benefits of using spread syntax and how is it different from rest syntax?  
answer:

### 59. How can you share code between files?  
answer:

### 60. Why you might want to create static class members?  
answer:
