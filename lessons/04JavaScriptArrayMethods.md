- [V2 Scrimba - JS Deep Dive - Objects & Maps](https://v2.scrimba.com/javascript-deep-dive-c0a/~01d)
- **NOTE: Watch only the rest of the videos in the playlist (the last 3 you were instructed to skip last week).**
  - **If you are getting an alert "Only available to subscribers" you will need to be sure your are logged in to Scrimba with the email address we have on file for you, and that you have redeemed the link to free access you were emailed.  Remember to start at the 9th part titled "How Maps can do what Objects can't" and go to the end of the Objects section**

- The section on "Intermediate/advanced array magic" that you could skip in last week's Odin Project Fundamentals part 5 is now included in the following section for you to check out this week:

> ### Intermediate/advanced array magic
>
> Besides being a quick and handy way to store data, arrays also have a set of functions for manipulating that data in very powerful ways. Once you begin to master these functions you will start to see ways to use them all over the place! There are really only a handful of these functions… but as you’ll soon see, the possibilities of what you can do with them are near endless.
>
> 1. Start out by watching [this video](https://www.youtube.com/watch?v=HB1ZC7czKRs) from Wes Bos. To follow along, use your local Javascript30 repository. If you don’t have the repo yet, clone it from [here](https://github.com/wesbos/JavaScript30).
> 2. Watch and code with [Part 2](https://www.youtube.com/watch?v=QNmRfyNg1lw) of Wes Bos’s array series.
> 3. For a more comprehensive and in-depth guide to array methods in JavaScript, you can also check out this [array method guide](https://javascript.info/array-methods). This resource covers each method in detail, with examples and explanations of their usage.

# Callbacks

Callbacks are functions that you provide to another function or system to be executed when a certain condition or event occurs. They are a way of saying, "Hey, when this thing happens, do this specific task.”

Imagine you have a button on a website, and you want something to happen when the button is clicked. You could create a callback function that specifies what should happen when the button is clicked. This callback function is then associated with the button.

```jsx
// A function that adds two numbers and uses a callback to return the result
function addNumbers(a, b, callback) {
  const result = a + b;
  callback(result);
}

// Define a callback function to handle the result
function handleResult(result) {
  console.log("The result is: " + result);
}

// Call the addNumbers function with a callback
addNumbers(5, 3, handleResult);
```

In this example, the **`addNumbers`** function takes two numbers **`a`** and **`b`**, adds them together, and then calls a provided **`callback`** function with the result. The **`handleResult`** function is the callback, and it prints the result to the console.

This demonstrates how callbacks can be used to pass control from one function to another, allowing you to specify what should happen after a specific operation (in this case, addition) is complete.

Watch this video on the mistake with functions every developer makes, because remember **making mistakes is a great way to learn!** [YouTube Video Link](https://www.youtube.com/watch?v=7UMuJMiNjSk&t=98s)

Callbacks are a versatile and powerful concept in programming, and they can be used in various scenarios. Here are some common situations where callbacks are useful:

1. **Asynchronous Operations:** Callbacks are often used with asynchronous operations, like making network requests, reading files, or interacting with databases. They allow you to specify what should happen when the operation is completed without blocking the rest of your program.
2. **Event Handling:** In user interfaces, callbacks are used to respond to user interactions such as button clicks, mouse movements, or keyboard input. You define a callback function that gets triggered when the event occurs.
3. **Modular and Reusable Code:** Callbacks make it easier to write modular and reusable code. You can create functions that accept callbacks to perform specific tasks, allowing you to reuse those functions with different behaviors depending on the callback provided.
4. **Iterations and Loops:** Callbacks can be used in iterations and loops to execute a function for each element in a collection, like an array or a list. This is known as "callback-based iteration."
5. **Promises and Promisified Code:** In JavaScript, promises often work with callbacks to handle asynchronous tasks more cleanly. Promises provide a structured way to handle callbacks and make asynchronous code easier to read and maintain.

Overall, callbacks are a fundamental building block in software development, enabling you to define what should happen when a particular event or operation occurs, making your code more flexible, modular, and responsive.

We will be covering all these aspects of the uses of callbacks in later lessons, but it is important to understand how they work at a very basic level.

# Higher Order Functions

As we talked about callbacks previously, higher-order functions are those functions that receive a callback as a parameter.

```jsx
function addNumbers(a, b, callback) {
  const result = a + b;
  callback(result);
}
```

You can create your own higher-order functions or you can use many of the built-in higher-order methods that are part of the Array object.

Arrays have many methods and one category of methods it has are iterative which means they will iterate through the array and execute the callback function you pass to it for every element in the array.

Examples would be the [forEach()](https://javascript.info/array-methods#iterate-foreach), [map()](https://javascript.info/array-methods#map), [filter()](https://javascript.info/array-methods#filter), and others.

### The forEach() method

The forEach() method accepts a function as an argument. The function that you pass to the method is referred to as a **callback** function. 

You provide forEach() with a callback function. Then, internally, forEach() executes that callback function once for each element of the array. 

```jsx
const numbers = [1, 2, 3, 4];
numbers.forEach(function(num) {
  console.log(num);
});
// This will print each number in the array.
```

### The map() method

The map() will run the callback function for each of the items in the array. The map() method uses the callback function to create the items for a new array. The map() method will return a new array of the same number of elements as the original array and the forEach method will not return anything.

```jsx
const numbers = [1, 2, 3, 4];
const squared = numbers.map(function(num) {
  return num * num;
});
// squared is now [1, 4, 9, 16]
```

### The filter() method

Sometimes, you'll want to build up a new list of items that meet a particular condition. This method builds a new array of only the items that match a certain condition. The filter() method will “filter” the array so that you have only some of the items.

```jsx
const numbers = [1, 2, 3, 4, 5, 6];
const evenNumbers = numbers.filter(function(num) {
  return num % 2 === 0;
});
// evenNumbers is now [2, 4, 6]
```

**Note:**  There are many more of these type of methods, but do not worry about knowing how to use all of them, starting with a few is good enough.
