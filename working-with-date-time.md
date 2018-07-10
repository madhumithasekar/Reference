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
