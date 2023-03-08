# using get method to send a response to the listening server
``` js
app.get('/',function(req,res)

{
    res.send('<h1>'+'this is Prabhu R'+'</h1>');
}

)

```

# difference between res.send and res.write

``` js
app.get('/write',function(req,res)

{
    res.write('<h1>'+'this is Prabhu R'+'</h1>');
     res.write('my armpit smells good');
     res.send();
}

)
```
## note: you can use many res.write() with res.send() method at end of it but res.send() method can be used only once