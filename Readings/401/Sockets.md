# Socket.io

## What is a websocket?
Websocket is a computer communication protocol (like https) that provides full-duplex communication channels over a single TCP connection. This protocol is located on 'layer 7' Sockets provide streams of information to those listening.

## socket.io
realtime bidirectional event-based communication. It works on every platform or browser or device. Socket.io  is built on top of the websockets api, and node.js. 

sockets are great for instant messages, push noticiations, collaboration applications, or online gaming. almost all online games are real-time.

sockets are bidirectional beaning server can push messages to clients, whenever an event occurs. this allows the server to recieve and push the requests to the concerned connected clients. 
```js
npm install --save express socket.io
```

```js
var app = require('express')();
var http = require('http').Server(app);
var io = require('socket.io')(http);

app.get('/', function(req, res){ res.sendFile('E:/test/index.html');
});

//Whenever someone connects this gets executed
io.on('connection', function(socket){
   console.log('A user connected');
   
   //Whenever someone disconnects this piece of code executed
   socket.on('disconnect', function () {
      console.log('A user disconnected');
   });
});
```

```js
!DOCTYPE html>
<html>
   <head><title>Hello world</title></head>
   <script src="/socket.io/socket.io.js"></script>
   <script>
      var socket = io();
   </script>
   <body>Hello world</body>
</html>
A user connected
A user disconnected
A user connected
```
[Doc important for socket implementation if need help](https://www.tutorialspoint.com/socket.io/socket.io_event_handling.htm)
[Broadcasting](https://www.tutorialspoint.com/socket.io/socket.io_broadcasting.htm)
[Live chat rooms](https://www.tutorialspoint.com/socket.io/socket.io_rooms.htm)

## key featues of web sockets

WebSocket helps in real-time communication between the Client and the webserver.
This protocol helps in transforming to cross-platform in a real-time world between the server and the client.
This also enables the business worldwide for a real-time web application to enhance and increase the feasibility.
The major advantage it stands over an HTTP connection that it provides full-duplex communication.

## key features of socket.io
It helps in broadcasting to multiple sockets at a time and handles the connection transparently.
It works on all platform, server or device, ensuring equality, reliability, and speed.
It automatically upgrades the requirement to WebSocket if needed.
It is a custom real-time transport protocol implementation on top of other protocols.
It requires both libraries to be used Client side as well as a server-side library.
IO works on work-based events. there are some reserved events that can be accessed using the Socket on the server side like Connect, message, Disconnect, Ping and Reconnect.
There are some Client based reserved events like Connect, connect- error, connect-timeout and Reconnect etc.
I handle all the degradation of your technical alternatives to get full-duplex communication in real-time.
It also handles the various support level and the inconsistencies from the browser.
It also gives the additional feature room support for basic publish infrastructure and thinks like automatic reconnect.
Currently, AFAIK is the most used one and easier to help with vanilla web sockets.

[CONTENT ABOVE IS FROM](https://www.educba.com/websocket-vs-socket-io/)

[Docs for implementation intro](https://socket.io/docs/v4/)
[Docs for implementation server API](https://socket.io/docs/v4/server-api)
[Docs for implementation server CLIENT API](https://socket.io/docs/v4/client-api)
[SOCKET IO TESTING TOOL](https://amritb.github.io/socketio-client-tool/)
