# Putting it all together

- What is the single responsibility principle and how does it apply to components?

>A component should only ever have one job, if its doing more than one thing, decompose into smaller subcomponents

- What does it mean to build a ‘static’ version of your application?

>Build a version of the app without interactivity as interactivity is not hard to implement while static implementations are

- Once you have a static application, what do you need to add?

>figure out absolute minimal representation of the state your application needs andcompute everthing else you need on-demand. 

- What are the three questions you can ask to determine if something is state?

>is it passed in from parent via props? not state (problably)
> > does it remained unchanged over time? (prob not state)
> > > can you compute it based on any other state or props in your component? if yes its not state babooshka

- How can you identify where state needs to live?

>where is the data changing? what other component needs this data? the common parent of those two components

- What is a “higher-order function”?

>Functions that operate on other functions either by taking them as args or by returning them; higher order functions.

- Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?

>return true or false if m is greater than n

- Explain how either map or reduce operates, with regards to higher-order functions.

>The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.
>It builds a value by repeatedly taking a single element from the array and combining it with the current value. When summing numbers, you’d start with the number zero and, for each element, add that to the sum.
