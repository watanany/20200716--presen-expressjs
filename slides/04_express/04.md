##  Expressとテンプレートエンジン

```javascript
app.get("/", function(req, res, next) {
    res.render("index", { title: "Express" });
});
```


```html
doctype html
html
    head
        title= title
    body
        p About Template Engine
```

