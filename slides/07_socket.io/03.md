app.js
```javascript
express = require('express');
app = express();

// ...

app.io.on('connection', function(socket) {
  // Socket.IOを使った処理
});

module.exports = app
```
