# javascript-interview-Questions

Question 1: What is the difference between .map() and .forEach()?
Answer:

.map() and .forEach() are both array methods that allow you to loop through an array, but they differ in what they return.

.map() returns a new array with the same length as the original array, where each element is the result of applying a callback function to the original element.
.forEach() does not return anything, but it simply executes a callback function on each element of the array.
Example:

const numbers = [1, 2, 3, 4, 5];

const doubledNumbers = numbers.map(num => num * 2);

console.log(doubledNumbers); // [2, 4, 6, 8, 10]

numbers.forEach(num => console.log(num * 2)); // 2, 4, 6, 8, 10


Question 2: What is the difference between .filter() and .find()?
Answer: Both .filter() and .find() are array methods that allow you to search for elements in an array that meet certain criteria.

.filter() returns a new array with all elements that pass a certain test provided by a callback function.
.find() returns the value of the first element in the array that passes a certain test provided by a callback function.
Example:

const numbers = [1, 2, 3, 4, 5];

const evenNumbers = numbers.filter(num => num % 2 === 0);

console.log(evenNumbers); // [2, 4]

const firstEvenNumber = numbers.find(num => num % 2 === 0);

console.log(firstEvenNumber); // 2

In this example, we use the .filter() method to create a new array with only the even numbers in the numbers array. We use the .find() method to return the first even number in the numbers array.
