----- Why we use meta tags? ------

In HTML, meta tags are used to provide metadata about a document. Commonly used meta tags include those that define the character set (<meta charset="UTF-8">), set the viewport for responsive design (<meta name="viewport" content="width=device-width, initial-scale=1.0">), and provide information for search engines (<meta name="description" content="Brief description of the page">).

----- Difference between pseudo class and pseudo elements in css -----

Pseudo-classes enable you to target an element when it's in a particular state, as if you had added a class for that state to the DOM. Pseudo-elements act as if you had added a whole new element to the DOM, and enable you to style that.

(Pseudo-classes are used to style elements based on their state or position in the document)
(Pseudo-elements allow you to style specific parts of an element, such as the first line or first letter.)

----- Difference beetwen Mixin and Extend in css -----

1 - A mixin is a way to group and reuse a set of CSS declarations.

@mixin border-radius($radius) {
  border-radius: $radius;
}

// Using the mixin
.box {
  @include border-radius(5px);
}

.button {
  @include border-radius(10px);
}

2 - Extend is a feature that allows one selector to inherit the styles of another.

.base-style {
  color: blue;
  font-size: 16px;
}

.header {
  @extend .base-style;
  font-weight: bold;
}

----- JS Data Types -----

1 -- Primitive ( string, number, boolean, undefined, null, symbol, BigInt) -(Single value)
2 -- Reference (Object(object, array, function...etc)) -(multiple value)

----- JS Variables difference -----

let myNumber = 42; Ozgaradigan o'zgaruvchi
var smth = true;   Global o'zgaruvchi
const str = 81;    O'zgarmaydigan o'zgaruvchi

----- Number methods  in JS -----

Number()
parseInt()
parseFloat()

----- Math object in JS -----

The Math object in JavaScript provides a set of properties and methods for mathematical operations. Here are some commonly used features of the Math object:

Math Constants:

Math.PI: Represents the mathematical constant Pi (π).
Math.E: Represents the mathematical constant Euler's number (e).

Math Methods:

Math.abs(x): Returns the absolute value of a number.
Math.sqrt(x): Returns the square root of a number.
Math.pow(x, y): Returns the value of x to the power of y.
Math.floor(x): Returns the largest integer less than or equal to a given number.
Math.ceil(x): Returns the smallest integer greater than or equal to a given number.
Math.round(x): Returns the value of a number rounded to the nearest integer.
Math.random(): Returns a pseudo-random number between 0 (inclusive) and 1 (exclusive).

----- String methods -----

length: Returns the length of a string.

let str = "Hello, World!";
console.log(str.length); // Output: 13

toUpperCase and toLowerCase:

toUpperCase(): Converts the string to uppercase.
toLowerCase(): Converts the string to lowercase.

let str = "JavaScript";
console.log(str.toUpperCase()); // Output: "JAVASCRIPT"
console.log(str.toLowerCase()); // Output: "javascript"

trim(): Removes whitespace from both ends of a string.

----- Difference between undifined and null -----

undefined means a variable has been declared but has not yet been assigned a value, whereas null is an assignment value, meaning that a variable has been declared and given the value of null .

----- Truthy, Falthy ------

In JavaScript, values are categorized as either "truthy" or "falsy" when evaluated in a boolean context (such as an if statement or as a condition in a loop). Understanding truthy and falsy values is important for writing conditional logic.

Falsy values:
Values that are considered falsy when coerced to a boolean are:

false: The boolean value false.
0: The number zero.
-0: Negative zero.
0n: BigInt zero.
"": An empty string.
null: The absence of a value.
undefined: A variable that has not been assigned a value.
NaN: Not a Number.

Truthy values:
Values that are considered truthy when coerced to a boolean are:

true: The boolean value true.
Any non-zero number (including negative numbers and decimals).
Any non-empty string.
An object (including arrays and functions).
The special value Infinity.
The special value -Infinity.
The special value NaN (though it's generally better to avoid relying on NaN truthiness).