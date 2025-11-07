# swe-sr-1-3

## Setup

For guidance on setting up and submitting this assignment, refer to the Marcy lab School Docs How-To guide for [Working with Short Response and Coding Assignments](https://marcylabschool.gitbook.io/marcy-lab-school-docs/how-tos/working-with-assignments#how-to-work-on-assignments).

Here are some useful commands to remember.

```sh
npm i                   # install dependencies
git checkout -b draft   # switch to the draft branch before starting

git add -A              # add a changed file to the staging area
git commit -m 'message' # create a commit with the changes
git push                # push the new commit to the remote repo
```
## Question 1

Read the documentation for `findIndex` and `indexOf` on MDN:
- [findIndex](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/findIndex)
- [indexOf](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/indexOf). 

Explain the difference between the methods and explain when you would choose one over the other. Provide examples to enhance your response.

### Response

Add your response here...

- We have **findIndex** in JS and it's only used in an array. 
- It takes certain condition and it will return the first condtion where it maches the **findIndex()** method. 
- I would choose this method to find values quicker because it take a condition. 
- It returns the first value that maches the condition. If it doesn't match the condition it'll return -1. 
- According MDN, this is the definition, "The findIndex() method of Array instances returns the index of the first element in an array that satisfies the provided testing function. If no elements satisfy the testing function, -1 is returned" 

*Here is an example for it:* 
```js 
const cars = [
    { name: 'BMW', year: 2025 },
    { name: 'Lambo', year: 2026 },
    { name: 'Honda', year: 2020 }
]
users.findIndex(car => car.name === "BMW") // it returns first index that matches the name "BMW"
users.findIndex(car => car.name === "Benz") // it will return -1. 

```
**


- There is a built-in method in JavaScript that called **indexOf** which is used to find the specific index of a value in a either a string or in an array. 

- It comes in handy when we want to find where the elements are in a big array or a long sentence. 
- If the value is not found in the array or in a string it returns -1, which means it doesn't exist there. 
According to MDN, this is what it says about how to find the indexOf, "The indexOf() method compares searchElement to elements of the array using strict equality."
- I would choose **indexOf()** if I have a big array or a long sentence, so that way I can find in what index the value is saved and located. 
*Here is how to use it:*
```js
const cars = ["BMW", "Camery gts 2026, V6, 350HP", "Benz", "Ford"]
cars.indexOf("Camry gts 2026, V6") // The out put would be 1. 
cars.indexOf("Lambo"); // returns -1 
```
