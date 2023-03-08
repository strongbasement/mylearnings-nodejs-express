# create a form.html near app.js

``` html
<form action="/form" method='post'>

<input type="text" name="name1">
<input type="email" name="email" id="ss">
<input type="submit" value="post">

</form>

```
## note : do not forget to declare method='post' in form


# let write the post method in the server wait before writting the method install body-parser npm package to parse input data from the form into the server

```
npm install body-parser

```
# declaring variable inside server 

``` js

const bodyparser=require('body-parser');

```
# use to encode url app.use config after declaring body parser variable

``` js
app.use(bodyparser.urlencoded({extended:true}));

```

# let write post method inside app.js server

``` js

app.post('/form',function(req,res)

{
var name=req.body.name1; /*storing input type name field value in a variable called. req is request to body ie form.html;body is bodyparser function;name1 is input type name mentioned while in form creation */ 
var email=req.body.email;
res.write('your name is '+name+' and your email is '+email);
res.send();
}


)
```
## note: form action and app.post root folders are same ie:
```
app.post('/form',function(req,res){...}) = <form action="/form">...</form> 
//do not copy justfor understanding
```
