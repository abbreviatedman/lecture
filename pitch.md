---
theme: league
---

# You Deserve Arrays

#### by Colin Jaffe

Not the array lecture you _want_, but the array lecture you _need_.

---

### Learning Objectives

- Explain why we need arrays.
- Create arrays.
- Connect array values with their indices.
- Loop through arrays.

---

### Why Arrays?

Arrays are there so that you don't have to make a new variable for every value in a list.

```javascript
// With a variable for every person:
const person1 = "Colin";
const person2 = "Miggy";
const person3 = "Sue";

// With ONE variable, an array:
const people = ["Colin", "Miggy", "Sue"];
```

We can also loop through an array just like a string--more on that soon!

---

### Arrays are collections just like strings

Strings are collections of characters.

```javascript
"hello"[0]; // --> 'h'
"hello"[4]; // --> 'o'
```

You don't often need to single out a character of a string. Arrays are _more useful collections_--they can hold _anything_.

Words, sentences, numbers, booleans... whatever you want!

```javascript
const data = ["my", "mental", "age", "is", 12, true];
data[0]; // --> 'my'
data[4]; // --> 12
data[5]; // --> true
```

---

### A closer look at that syntax

```javascript
// Creating an array with values in it.
// Storing it in a variaable called `people`.
const people = ["Emily", "Jay", "Maria", "Miggy", "Sue"];

// Accessing values by index:
people[2]; // --> 'Maria"

// Using an array literal--not too common, but you don"t _have_
// to put it in a variable!
["Emily", "Jay", "Maria", "Jose", "Sue"][2]; // "Maria"
```

---

### Arrays As Streets

You can think of an array as a street:

- It's a collection of houses with addresses.
- Each house has something inside it (the value at that address).
- You can walk down the street. (A loop!)

---

### Array Street - Visualized

```javascript
const mainStreet = ["Emily", "Jay", "Maria", "Miggy", "Sue"];
/*
 ____       ____       ____       ____       ____
/     \    /     \    /     \    /     \    /     \
|Emily|    | Jay |    |Maria|    |Miggy|    | Sue |
   0          1          2          3          4
*/
```

---

### We can look up who lives at the house if we know:

1. the street
2. the address

```javascript
const mainStreet = ["Emily", "Jay", "Maria", "Miggy", "Sue"];
/*
 ____       ____       ____       ____       ____
/     \    /     \    /     \    /     \    /     \
|Emily|    | Jay |    |Maria|    |Miggy|    | Sue |
   0          1          2          3          4
*/

mainStreet[1]; // --> "Jay"
mainStreet[4]; // --> "Sue"
```

---

### We can also loop through arrays

This is the equivalent of walking down the street, checking every house.

```javascript
for (let i = 0; i < mainStreet.length; i++) {
  console.log("Hello, " + mainStreet[i] + "!");
}

/*
Prints out:
"Emily"
"Jay"
"Maria"
"Miggy"
"Sue"
*/
```

You'll notice it's the exact same syntax as with strings. But now we're getting full values, not just characters!

---

### And now let's try them out!

You now have arrays. _You're welcome._
