# Passing functions as props

- What does .map() return?

>map returns a new array consisting of data modified from a passed array through a callback function or operation.

- If I want to loop through an array and display each value in JSX, how do I do that in React?

>See code example

```js
const listItems = numbers.map((number) =>
  <li>{number}</li>
);
```

- Each list item needs a unique ____.

>Key value

- What is the purpose of a key?

>Keys help react identify which items have changes are added or are removed. keys should be given to elements inside the array to give the elements a stable identity

- What is the spread operator?

>The spread operator allows an expression to be expanded in places where multiple arguments (for function calls) or multiple elements (for array literals) are expected.

- List 4 things that the spread operator can do.

>function calls, array literals, destructuring, array prototype methods?

- Give an example of using the spread operator to combine two arrays.

```js
const a = [1, 2, 3]
const b = [...a, 4] // b ==> [1, 2, 3, 4]
```

>example above

- Give an example of using the spread operator to add a new item to an array.

```js
let numberStore = [0, 1, 2];
let newNumber = 12;
numberStore = [...numberStore, newNumber];
```

>see above

- Give an example of using the spread operator to combine two objects into one.

```js
let person = {
    firstName: 'John',
    lastName: 'Doe',
    age: 25,
    ssn: '123-456-2356'
};


let job = {
    jobTitle: 'JavaScript Developer',
    location: 'USA'
};

let employee = {
    ...person,
    ...job
};

console.log(employee);
```

>See above

- In the video, what is the first step that the developer does to pass functions between components?

>create function where state needs to be changed, indentifys why he needs a function and where

- In your own words, what does the increment function do?

>the incriment function takes in an object, copys it, and modifies the value of property count on one of the objects if conditions are met. further more on the person component incriment just flips a property value to true/positive based on input.

- How can you pass a method from a parent component into a child component? 

>as any other prop, through the object in the parent object

- How does the child component invoke a method that was passed to it from a parent component?

>
```js
this.props.method_name_from_parent(params needed for the method name)
```



<https://www.javascripttutorial.net/object/javascript-merge-objects/>
