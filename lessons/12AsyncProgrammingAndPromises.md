Go through **both** resources (Odin **and** Scrimba) for this topic as they will help you gain a more clear understanding of this topic.

Remember to please go to each link in this list and read through the content on that page. If there are links you are redirected to as you read/work through the content, follow those links as well and read the content there too.

- **[The Odin Project – Asynchronous Code](https://www.theodinproject.com/lessons/node-path-javascript-asynchronous-code)**
- **[Scrimba - JavaScript Deep Dive - Async JS - Fix Callback Hell with Promises](https://v2.scrimba.com/javascript-deep-dive-c0a/~02o)**
- **[Scrimba - Introduction to ES6+ - Promises](https://v2.scrimba.com/introduction-to-es6-c0t/~0q)**
- **[Scrimba - Introduction to ES6+ - Challenge: Promises](https://v2.scrimba.com/introduction-to-es6-c0t/~0r)**

## Synchronous vs. Asynchronous code

*Synchronous code* executes one code instruction at a time, in the order that the instructions are given. *Asynchronous code* executes multiple instructions simultaneously, and the order in which the instructions are completed isn't known. 

With asynchronous code, multiple tasks can be executed at the same time while tasks in the background finish. This is what we call *non-blocking* code. The execution of other code won't stop while an asynchronous task finishes its work.

```jsx
let greet_one = "Hello"
let greet_two = "World!!!"
console.log(greet_one)
setTimeout(function(){
    console.log("Asynchronous");
}, 10000)
console.log(greet_two);
```

In the above example, if you run the code on your machine you will see `greet_one` and `greet_two` logged even if there is code in between those 2 logs.

Now, setTimeout is asynchronous so it runs in the background, allowing code after it to execute while it runs. After 10 seconds, `Asynchronous` will print because we set a time of 10 seconds in setTimeout to execute it after 10 seconds.

1. Read this article about [synchronous and asynchronous](https://www.telerik.com/blogs/how-javascript-code-gets-executed-synchronous-asynchronous)

[Watch this video on Async vs Sync](https://www.youtube.com/watch?v=wYRw8f-wrco&t=253s)

## Promises

When it comes to handling asynchronous code, the go-to tool is something called a **promise**. This nifty object can handle async tasks and gives you a bunch of methods to neatly pluck out a single result.

Here's the deal: Asynchronous code can be a bit of a puzzle because it messes with the usual order of things. It can get pretty tricky in some situations.

But that's where promises come to the rescue! They're like a protective wrapper around async code. Promises are smart – they won't trigger the callback function until it's absolutely necessary. Plus, they hand you some nifty functions to deal with whatever outcome your async code delivers, whether it's a triumphant success or a less-than-ideal failure.

```jsx
const newPromise = new Promise((resolve, reject) => {
  // Your code here...
});
```

A new promise can be created using the **new** keyword with the [Promise](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/Promise) class. This will create an instance of a promise. Promises can be assigned to variables. The only argument to pass into the Promise constructor is a callback function that has two parameters: **resolve** and **reject.**

To manage asynchronous code, promises have **three states:**

- **Pending:** When a promise is first created, it has a status of *pending*.
- **Fulfilled:** When the promise has successfully finished running, it has a status of *fulfilled*. This means that it is ready to pass back a value.
- **Rejected:** If something goes wrong, the promise changes to a status of *rejected*. This means that something failed.

### Resolving Promises

Now that you've got the hang of creating promises, you might have noticed something missing – a way to snoop on a promise's mood, like whether it's feeling "pending," "fulfilled," or "rejected." There's also no direct way to peek at what the promise has decided to resolve to or why it's throwing a fit.

Unlike your typical JavaScript objects, promises are like chameleons. They can switch between their states (and values) from pending to fulfilled or rejected whenever they please. This means you've got to keep an eye on them.

So, here's the deal: Promises rely on callback functions to raise a flag when their state changes. 

When the promise is all smiles and gets resolved, it'll call the callback function hanging out in the **`then()`** method and share its resolved value. But if it's having a bad day and gets rejected, the **`catch()`** method swoops in, bringing along the rejected reason (aka, the error). 

It's like a promise's way of saying, "Hey, something happened, and here's what went down!"

### The then() method

When a promise is created, the asynchronous operation inside will be fulfilled as quickly as possible. However, there are no methods or properties available to directly access the resolved value of a promise.

The then() method accepts a callback function that is called whenever the promise is fulfilled. 

```jsx
// Creating a Promise
const myPromise = new Promise((resolve, reject) => {
  // Simulating an asynchronous task 
  setTimeout(() => {
    const data = "Here's the result!";
    resolve(data); // Resolving the promise with some data
  }, 2000); // Simulating a 2-second delay
});

// Using the Promise
myPromise.then((result) => {
  console.log("Promise resolved with data:", result);
}).catch((error) => {
  console.error("Something went wrong:", error);
});
```

1. We create a **`myPromise`** object using the **`Promise`** constructor. Inside the promise, we simulate an asynchronous task using **`setTimeout`**. After 2 seconds, the promise is resolved with the message "Here's the result!"
2. We use the **`then`** method to handle the resolution of the promise. When the promise is resolved, the provided callback function is executed, and it logs the resolved data.
3. If an error were to occur inside the promise (e.g., if we used **`reject`** instead of **`resolve`**), the **`catch`** method would handle the error and log it.

### **The catch() method**

The **`catch()`** method in JavaScript is like the safety net for promises. Just like how try/catch blocks work, if the **`catch()`** method doesn't throw an error itself, the function calling it won't know that something went wrong. In simple terms, the promise attached to **`catch()`** only becomes rejected if **`catch()`** encounters an error or returns a promise that also gets rejected. Otherwise, it resolves as if everything went smoothly.

![promise catch flow](https://github.com/Code-the-Dream-School/intro-to-programming-2024/blob/41a41459613b5c8e6cc3f9171feebfc1837b0c8e/Screenshot%25202023-09-24%2520at%252010.19.29%2520PM.png)

1. Read [this article about Promises](https://javascript.info/promise-basics)
2. Read [this second article about Promises](https://dmitripavlutin.com/what-is-javascript-promise/)

Watch these two short videos on JavaScript Promises:

1. [JS Promise in 100 Seconds](https://www.youtube.com/watch?v=RvYYCGs45L4)
2. [Async JS: Promises](https://www.youtube.com/watch?v=slIJj-zbs_M)
