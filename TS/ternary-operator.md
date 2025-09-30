The ternary operator is a concise way to write conditional logic in JavaScript/TypeScript. 
It's essentially a shorthand for an if-else statement.

```js
condition ? valueIfTrue : valueIfFalse
```

Evaluate condition: If it's truthy, use the first value
If condition is falsy: Use the second value

Good for:
Simple conditional assignments
Short, readable conditions
One-liner returns

Avoid for:
Complex logic
Multiple statements
When readability suffers

Simple Examples:

```ts
// Basic usage
const age = 20;
const status = age >= 18 ? "adult" : "minor";
// Result: "adult"

// With numbers
const score = 85;
const grade = score >= 90 ? "A" : score >= 80 ? "B" : "C";
// Result: "B"

// With boolean logic
const isLoggedIn = true;
const message = isLoggedIn ? "Welcome back!" : "Please log in";
// Result: "Welcome back!"
```

Nested Ternary (Chaining):
```ts
// Multiple conditions
const grade = score >= 90 ? "A" : 
              score >= 80 ? "B" : 
              score >= 70 ? "C" : 
              score >= 60 ? "D" : "F";

// Equivalent if-else chain:
let grade;
if (score >= 90) {
  grade = "A";
} else if (score >= 80) {
  grade = "B";
} else if (score >= 70) {
  grade = "C";
} else if (score >= 60) {
  grade = "D";
} else {
  grade = "F";
}
```


