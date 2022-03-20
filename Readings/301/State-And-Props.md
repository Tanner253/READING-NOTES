# What is state and what are props?

>props pass data from parent to child. must recieve data from the outside to update. State is managed inside the component, and can be updated within.  will re render the site on change.

## state vs props
>state is for rerending the application based on what the user has done. 
> > props are useful for when you want to display information without hardcoding it, essentially making it a variable that can be worked with dynamically

## when do I use state when do I use props?

>is information being handled inside or outside the component?
> > if its being handled AT ALL outside the component it should be props! (otherwise if its internal use state!)

### Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?

>Render

### What is the very first thing to happen in the lifecycle of React?

>Constructor is called

### Put the following things in the order that they happen:

>(they are now in order) constructor, render, React Updates, componentDidMoun, componentWillUnmount,

### What does componentDidMount do?

>"This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions. If you do that, don’t forget to unsubscribe in componentWillUnmount()"
<https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093>

### What types of things can you pass in the props?

>objects, Arrays, intigers, strings, pretty much anything.

### What is the big difference between props and state?

>props are used to pass data from one component to another. state is controlled within the component local storage that cannot be passed to other components

### When do we re-render our application?

>When the state of a component has changed or is updated

### What are some examples of things that we could store in state?

>we can store components in state, inputs, checkbox, timers much more