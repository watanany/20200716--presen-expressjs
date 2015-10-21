##  Node.jsのみでのルーティング

```javascript
server.on("request", function(req, res) {
	res.writeHead(200);
	if (req.url === "/") {
		res.write("Hello World!")
	}
	else if (req.url === "/test") {
		res.write("レスポンスしてみるテスト")
	}
	else {
		res.write("404 NOT FOUND");
	}
	// レスポンスを終了する
	res.end();
});

server.listen(setting.PORT, setting.IP, setting.startServer);
```
