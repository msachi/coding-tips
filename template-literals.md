Template literals are string literals that allow embedded expressions.

They are enclosed by the back-tick (`` ` ```` ` ``), rather than single or double quotes like normal strings. They can contain place holders, indicated by the Dollar sign (`$`) and curly braces (`{}`), which serve to embed expressions that are then evaluated and concatenated with the rest of the text into a single string.

Template literals make it easier to write multi-line strings, and allow substitutions in strings more readable.

Example using normal strings:

```javascript
numWords = 1000;
console.log("A picture\n" + "is worth a " + numWords + " words");
// 'A picture
// is worth a 1000 words'
```

Example using template literals:

```javascript
console.log(`A picture
is worth a ${numWords} words`)
// 'A picture
// is worth a 1000 words'
```

Template literals also allow _tagging_, which is a way of modifying their output using a custom function. The details on how to use tagging are beyond the scope of this TIL, but you can see the [MDN entry on template literals](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals) for more information.
