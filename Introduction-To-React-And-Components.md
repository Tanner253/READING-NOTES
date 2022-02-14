# What is React?

>React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

## How does arrow functions affect how a function is invoked?

"Notice how with onClick={() => console.log('click')},
 we’re passing a function as the onClick prop.
React will only call this function after a click.
 Forgetting () => and writing onClick={console.log('click')} is a common mistake,
  and would fire every time the component re-renders."
  <https://reactjs.org/tutorial/tutorial.html>


## when defining constructors

>you must always call super to define sublasses

- In JavaScript classes, you need to always call super when defining the constructor of a subclass. All React component classes that have a constructor should start with a super(props) call.

- <https://reactjs.org/tutorial/tutorial.html>


## Why immutable?

>Complex Features Become Simple
Immutability makes complex features much easier to implement. Later in this tutorial, we will implement a “time travel” feature that allows us to review the tic-tac-toe game’s history and “jump back” to previous moves. This functionality isn’t specific to games — an ability to undo and redo certain actions is a common requirement in applications. Avoiding direct data mutation lets us keep previous versions of the game’s history intact, and reuse them later.
>Detecting Changes
Detecting changes in mutable objects is difficult because they are modified directly. This detection requires the mutable object to be compared to previous copies of itself and the entire object tree to be traversed.
>Detecting changes in immutable objects is considerably easier. If the immutable object that is being referenced is different than the previous one, then the object has changed.
>Determining When to Re-Render in React
The main benefit of immutability is that it helps you build pure components in React. Immutable data can easily determine if changes have been made, which helps to determine when a component requires re-rendering.


```js
/*class Square extends React.Component {
  render() {
    return (
      <button 
        className="square" 
        onClick =  {() => this.props.onClick()}
        >
        {this.props.value}
      </button>
    );
  }
}
*/
function Square(props){
  return (
  <button className="square" onClick={props.onClick}>
      {props.value}
      </button>
  );
}
}
```

## what is JSX

Jsx is a syntax extension to javascript

## why JSX

instead of seperating technologies by puting markup and login in seperate files, react prefers to loosly couple units into compontents. also prevents injection attacks

- When we modified the Square to be a function component, we also changed onClick={() => this.props.onClick()} to a shorter onClick={props.onClick} (note the lack of parentheses on both sides).
- <https://reactjs.org/tutorial/tutorial.html>

What is a “component”?
>a small piece of UI.
What are the characteristics of a component?
>components manage their own state, recieve information from parents and pass down to children
What are the advantages of using component-based architecture?
>Reduces the cost of development and maintainence.
What is “props” short for?
>properties which are parameters passed into children components
How are props used in React?
>they carry information that is passed down from parent to child.
What is the flow of props?
>one way parent to child.

## Things I want to know more about:
> This syntax is still new to me so I want to get more comfortable with that.. The way state and this are used is really intuitive.
