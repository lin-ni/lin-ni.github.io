JavaScript Fundamentals

---

## Data Types

-   In JavaScript, `value` has a type, not `variable`.

```javascript
console.log(typeof true);
console.log(typeof javascriptIsFun);
console.log(typeof 23);
console.log(typeof "Jonas");
```

-   `null` type: `undefined`

```javascript
console.log(typeof null); // This is a bug in JavaScript, it is not an object, the type is actually undefined.
```

## `let`, `const` and `var`

-   `const`

```javascript
const birthYear = 1991;
// birthYear = 1992; // WRONG, const cannot be reassign.
// const birthYear; // WRONG, const must be initialized.
```

-   `let` is block scope, `var` is function scope
-   This works, but terrible! NEVER use it.

```javascript
lastName = "Schmdtmann";
console.log(lastName);
// This works, but terrible! NEVER use it.
```

## Basic Operators

-   `2**3` is `2^3` = `2 * 2 * 2`.
-   [MDN operator precedence][1]

```javascript
const isFullAge = ageSarah >= 18;
// isFullAge is boolean.
```

-   Assign two variables

```javascript
let x, y;
x = y = 10;
```

## Strings and Template Literals

-   Backticks

```javascript
// Before
const jonas =
    "I'm " + firstName + ", a " + (year - birthYear) + " year old " + job + "!";
console.log(jonas);

// After
const jonasNew = `I'm ${firstName}, a ${year - birthYear} year old ${job}!`;
console.log(jonasNew);

// Backticks can be used for all strings.
console.log(`Just a regular string...`);

console.log(
    "String with \n\
    multiple \n\
    lines"
);
// \n\ allows us to write the string in multiple lines.
```

## Type Conversion and Coercion

```javascript
console.log("23" - "10" - 3); // output: 10
console.log("23" + "10" - 3); // output: 2307
// minus: convert string to number
// add: convert number to string
```

## Truthy and Falsy Values

-   5 falsy values: `0`, `''`, `undefined`, `null`, `NaN`(number).

```javascript
let height = 0;
if (height) {
    console.log("YAY! Height is defined!");
} else {
    console.log("Height is UNDEFINED");
}

// However height is actually defined, this is a bug.
// Thoughts: if (height != null)
```

## Equality Operators: `==` vs. `===`

-   `===`: strict equal. eg: `18 === 18`, both type and value.

-   `==`: loose equal. eg: `"18" == 18`. Will perform type coercion

!> Always use `===`!

## Statements and Expressions

-   The statement performs an action. It does not produce a value.

```javascript
/* Expression */
3 + 4
1991
true && false && !false

/* Statements */
if (23 > 10) {
    const str = "23 is bigger";
}

console.log("I'm ${2037 - 1997} years old.") // Correct
console.log(${if (23 > 10) {const str = "23 is bigger";}}) // WRONG! Statements cannot be used here!

const me = "Jonas";
console.log("I'm ${me}"); // Correct
```

## The Conditional (Ternary) Operator

```javascript
const age = 23;
age >= 18
    ? console.log("I like to drink wine.") // if so
    : console.log("I like to drink water."); // else

/* If Statement */
if (age >= 18) {
    ("wine");
} else {
    ("water");
}

/* Expression */
age >= 18 ? "wine" : "water";

const drink = age >= 19 ? "wine" : "water"; // Correct!
console.log(drink);
```

[1]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Operator_Precedence
