# socket.io Chat example
[get started!](https://socket.io/get-started/chat/)

```js
const express = require('express');
const app = express();
const http = require('http');
const server = http.createServer(app);
const { Server } = require("socket.io");
const io = new Server(server);

app.get('/', (req, res) => {
  res.sendFile(__dirname + '/index.html');
});

io.on('connection', (socket) => {
  console.log('a user connected');
});

server.listen(3000, () => {
  console.log('listening on *:3000');
});
```
 We can integreate socket.IO in 2 parts, the server integreation above and the client library below 
 ```js
 <script src="/socket.io/socket.io.js"></script>
<script>
  var socket = io();
</script>
```

404'not founds