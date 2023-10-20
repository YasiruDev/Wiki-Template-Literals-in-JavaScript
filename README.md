# Working with Template Literals in JavaScript

JavaScript introduced a cool feature in ES6 called Template Literals. Instead of the old single or double quotes, we use backticks ` `` ` to enclose strings. This makes creating strings, especially with dynamic content, much easier. Now, let’s dive into some fresh examples of template literals! 😎🚀

**Basic String :**
Imagine greeting someone by name.

```javascript
const name = ‘Alice’;
const message = `Welcome back, ${name}!`;
console.log(message); // Output: Welcome back, Alice!
```

**Easy Multiline Strings:**
No more weird breaks in your strings.

```javascript
const poem = `
These literals,
Are super cool.`;
console.log(poem);

// Output :
`These literals,
Are super cool.`
```

**Mathematical Operations**

```javascript
const length = 7;
const width = 6;
const message = `The area is ${length * width}.`;
console.log(message); // Output: The area is 42.
```

**Tagged Templates:**
An advanced use-case, tagged templates, let you preprocess strings.

```javascript
function emphasis(words, …values) {
return `${words[0]}**${values}**!`;
}
const word = “cool”;
const shoutOut = emphasis`JavaScript is ${word}`;
console.log(shoutOut); // Output: JavaScript is **cool**!
```

**Using Backticks Inside:**
You can use backticks inside your strings easily.

```javascript
const tip = `Use \`backticks\` for these literals.`;
console.log(tip); // Output : Use `backticks` for these literals.
```

**Conditional Rendering with Ternary Operators:**
Switch up your string based on a condition.

```javascript
const age = 17;
const voteMessage = `You’re ${age >= 18 ? ‘good’ : ‘not good’} to vote.`;

console.log(voteMessage); // Output: You’re not good to vote.
```

**Making a List:**
Combine arrays, loops, and template literals for dynamic lists.

```javascript
onst pets = [‘Cat’, ‘Dog’, ‘Parrot’];
const petList = `
Pets:
${pets.map(pet => `- ${pet}`).join(‘\n ‘)}
`;
console.log(petList);

// output
`Pets:
- Cat
- Dog
- Parrot`
```
[Medium](https://medium.com/@shaluka.gayanath/working-with-template-literals-in-javascript-992b59b7540c)

Template literals have made it super easy to work with strings in JavaScript. You can easily include variables, calculations, and cool tricks in your strings. They make your code cleaner and easier to read, so give them a try!
