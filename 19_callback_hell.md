https://www.youtube.com/watch?v=yEKtJGha3yM&list=PLlasXeu85E9eWOpw9jxHOQyGMRiBZ60aX&index=2

1. "Time, tide and JS waits for none"
2. Callback function enables us to do async programming in JS. We use this for some functions that are interdependent on each other for execution. For eg: Ordering can be done after adding items in cart. So we pass cb functions as argument to functions which then call the cb function passed. However this causes some problems:
     a.) Callback Hell: When a callback function is kept inside another function, which in turn is kept inside another function. (in short, a lot of nested callbacks). This causes a pyramid of doom structure causing our code to grow horizontally, making it tough to manage our code.
     b.) Inversion of control: This happens when the control of program is no longer in our hands. In nested functions, one API calls the callback function received but we don't know how the code is written inside that API and how will it effect our code. Will our function be called or not? What if called twice? What if it has bogs inside it? We have given control of our code to other code. 
