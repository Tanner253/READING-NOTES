# EDD (Event driven development)

## EventEmitter

```js
const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;
```

we use the emit method to trigger the event.

```js
function login(username){
  chatRoomEvents.emit('userJoined', username);
}
```

## removing listeners
to remove listeners we can use the removeListerner or RemoveAllListeners method. this comes built with nose meaning you want to pass a reference to the function. it is a lot harder to remove listeners from anonymous functions.

```js
const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter;
```

```js
function userJoined(username){
  chatRoomEvents.on('message', function(message){
    document.write(message);
  })
}

chatRoomEvents.on('userJoined', userJoined);
```

All of that headache can be avoided if we rewrite the code like so:

```js

const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter;

function displayMessage(message){
  document.write(message);
}

function userJoined(username){
  chatRoomEvents.on('message', displayMessage);
}

chatRoomEvents.on('userJoined', userJoined);

```

Now if we want to remove the displayMessage function from the message event’s list of handlers:

```js

chatRoomEvents.removeListener('message', displayMessage);
```

OOP comes into play with EDD <3

## docs

[https://nodejs.org/api/events.html](Node docs for event functions)
