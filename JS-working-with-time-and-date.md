## To print Time
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

### Time methods

```javascript
var d = new Date();
d.toTimeString();
```

returns

"14:43:05 GMT-0700 (PDT)"

```javascript
d.toTimeString().substr(0,8) -> substring from 0 - 8 
```
returns

"14:43:05"

```javascript
d.getDate() -> returns 16

d.getMonth() -> returns 5

d.getHours() -> returns 14

d.getMinutes() -> returns 55
```

### To print a 24 hour clock

```javascript
c.innerHTML = d.getHours() + ':' + d.getMinutes();
```

### To print a 12 hour clock

```javascript
var d = new Date();

var hours = d.getHours();
if (hours > 12) {
  hours =-12;
}

c.innerHTML = hours + ':' + d.getMinutes();
```

