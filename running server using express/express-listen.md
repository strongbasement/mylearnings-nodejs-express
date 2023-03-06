### step 1 :npm install express
### step 2 :declare constants:
``` js

const express=require('express');
const app=express();
```
### step 3:make your server listen

``` js
app.listen(3000,function()
{
   console.log('server is running on port 3000'); 
}
);


```

### step 4 :open your terminal and type
```
nodemon yourjsfilename.js
```

### step 5 : output will look like this

![Alt text](__dirname+noder.png)

## step 6:complete source

``` js
const express=require('express');
const app=express();



app.listen(3000,function()
{
   console.log('server is running on port 3000'); 
}
);

```
