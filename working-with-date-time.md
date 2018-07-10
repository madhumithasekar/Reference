The below code prints the time

```javascript

document.addEventListener('DOMContentLoaded, function(){
   var c= document.getElementById('current-time');

   var d = new Date();
   
   //toTimeString() -> converts time to a readable format 
   c.innerHTML = d.toTimeString();

});
```

The above returns

14:34:36 GMT-0700 (PDT)

Time methods

var d = new Date();
d.toTimeString();

returns

"14:43:05 GMT-0700 (PDT)"

d.toTimeString().substr(0,8) -> substring from 0 - 8 

returns

"14:43:05"

