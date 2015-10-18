##  Expressによるルーティング

```javascript

app.get("/", function(req, res, next) {
    res.send("Hello World!")
});

app.get("/test", function(req, res, next) {
    res.send("レスポンスしてみるテスト");
});

app.use(function(req, res, next) {
    err = new Error("404 NOT FOUND");
    err.status = 404;
    next(err);
});


```
