https://www.youtube.com/watch?v=U74BJcr8NeQ&list=PLlasXeu85E9eWOpw9jxHOQyGMRiBZ60aX&index=4

1. Promise can be created using a ```new Promise()``` constructor function.
2. This constructor function takes a callback function as argument. 
3. The callback function has 2 arguments named ```resolve``` and ```reject```. Resolve and reject are the keywords provided by JS.
4. We can only resolve or reject a promise. Nothing else can be done.
5. An error can also be created using ```new Error('error message')```.
6. There is also ```.catch()``` which is used to attach a failure callback function that handles any error that pops up during the execution of promise chain.
7. ```.catch``` only handles error of ```.then()``` that are present above it. If there is any ```.then()``` below it, catch will not handle any error for that, also that ,then will get executed no matter what.
8. It can be useful in a way if we want to catch error for a particular portion of a chain.
9. We can have multiple catch based on requirement and then a general catch at the end.
10. Always remember to return a value in the promise chain for the next ```.then``` to use ```.```
11. If it returns a value => It will be  used as an argument in next function. If it is a promise then the next ```.then``` in the promise chain is attached to the promise returned by the current callback function.
