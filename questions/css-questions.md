
### 1. What is CSS selector specificity and how does it work?
answer:  
soooooo. CSS selecor is basically a pattern used to select elements you want to style.
How does it work? you just type something like that:

```css
.selector {
    background-color: black;
}
```

and the `<div class="selector">` will aquire properties typed in css file.

there are some other selector types and how to type them

| Selector        | Example           | Example description         |
| --------------- |:-----------------:| ---------------------------:|
| .class          | .intro          | Selects all elements with class="intro" |
| ###id             | ###firstname      |   Selects all elements with id="firstname" |
| *               | *               |   Selects all elements             |
| element         | p               |   Selects all `<p>` elements             |
| element,element | div,p           |   Selects all elements and all `<p>` elements            |
| element element | div p           |   Selects all `<p>` elements inside `<div>` elements            |
| element>element | div > p         |   Selects all `<p>` elements where parent is a `<div>` element          |
| element+element | div + p         |   Selects all `<p>` elements that are placed immediately after `<div>` elements             |
| element1~element2| p ~ ul         |   Selects every `<ul>` element that are preceded by a `<p>` element             |
| [attribute]     | [target]        |   Selects all elements with a target attribute             |
| [attribute=value]| [target=_blank]|   Selects all elements with target="_blank"            |
| :active         | a:active        |   Selects the active link            |
| ::after         | p:after         |   Inserts something after the content of each `<p>` element             |
| ::before        | p:before        |   Inserts something before the content of each `<p>` element             |
| :checked        | input:checked   |   Selects every checked `<input>`            |
| :disabled       | input:disabled  |   Selects every disabled `<input>`            |
| :enabled        | input:enabled   |   Selects every enabled `<input>`            |
| ::first-letter  | p::first-letter |   Selects first letter of every `<p>` element            |
| ::first-line    | p::first-line   |   Selects first line of every `<p>` element            |
| :hover          | a:hover         |   Selects links on mouse hover            |
| :invalid        | input:invalid   |   Selects invalid `<input>` elements            |
| :link           | a:link          |   Selects all unvisited links            |
| :optional       | input:optional  |   Selects all optional inputs            |
| :in-range       | input:in-range  |   Selects `<input>` elements with a value within a specified range            |
| :out-of-range   | input:out-of-range|   Selects `<input>` elements with a valute outside a specified range            |
| :read-only      | input:read-only |   Selects `<input>` elements with the 'readonly' attribute specified            |
| :read-write     | input:read-write|   Selects `<input>` elements with the 'readonly' attribute not specified           |
| ::selection     | ::selection     |   Selects portion of an element that is selected by a user            |
| :target         | ###news:target    |   Selects the current active ###news element (clicked on a URL containing that anchor name)            |
| :valid          | input:valid     |   Selects all input elements with a valid value            |
| :visited        | a:visited       |   Selects all visited links            |

### 2. What's the difference between "resetting" and "normalizing" CSS? Which would you choose, and why?
answer:
First of all what the heck are those "reset" and "normalization" in CSS? Well, most browsers currently in use (actually all I am aware of) have some starter styles. For example links on most of them are blue. So to get rid of this styles you should reset them. This is where Reset and Normalize comes. Both of them works quite the same and simple, but Normalize also removes browser inconsistencies for HTML and preserve some useful defaults. Normalize is called by some "the new reset". 
Also i prefer Normalize.css cause its easier to install it via npm.


### 3. Describe Floats and how they work.
answer:
Floats are properties used to stick elements to the sides of their containers.
For example:
```css
a {
    float: right;
    /* the a element is stuck to the right  */
}
```

### 4. Describe z-index and how stacking context is formed.  
answer:
z-index is something-like z axis. So an element with greater z-index value is always in front of a object with lower z-index value
```css
img {
    float: left;
    z-index: -1;
}
/* this image will always be below the text */
```

### 5. Describe BFC(Block Formatting Context) and how it works.
answer:



### 6. What are the various clearing techniques and which is appropriate for what context?
answer:



### 7. How would you approach fixing browser-specific styling issues?
answer:


### 8. How do you serve your pages for feature-constrained browsers?
answer:


### 9. What techniques/processes do you use?
answer:


### 10. What are the different ways to visually hide content (and make it available only for screen readers)?
answer:


### 11. Have you ever used a grid system, and if so, what do you prefer?
answer:


### 12. Have you used or implemented media queries or mobile specific layouts/CSS?
answer:


### 13. Are you familiar with styling SVG?
answer:


### 14. Can you give an example of an @media property other than screen?
answer:


### 15. What are some of the "gotchas" for writing efficient CSS?
answer:


### 16. What are the advantages/disadvantages of using CSS preprocessors?
answer:


### 17. Describe what you like and dislike about the CSS preprocessors you have used.
answer:


### 18. How would you implement a web design comp that uses non-standard fonts?
answer:


### 19. Explain how a browser determines what elements match a CSS selector.
answer:


### 20. Describe pseudo-elements and discuss what they are used for.
answer:


### 21. Explain your understanding of the box model and how you would tell the browser in CSS to render your layout in different box models.
answer:


### 22. What does * { box-sizing: border-box; } do? What are its advantages?
answer:


### 23. What is the CSS display property and can you give a few examples of its use?
answer:


### 24. What's the difference between inline and inline-block?
answer:


### 25. What's the difference between a relative, fixed, absolute and statically positioned element?
answer:


### 26. What existing CSS frameworks have you used locally, or in production? How would you change/improve them?
answer:


### 27. Have you played around with the new CSS Flexbox or Grid specs?
answer:


### 28. Can you explain the difference between coding a web site to be responsive versus using a mobile-first strategy?
answer:


### 29. Have you ever worked with retina graphics? If so, when and what techniques did you use?
answer:


### 30. Is there any reason you'd want to use translate() instead of absolute positioning, or vice-versa? And why?
answer:


