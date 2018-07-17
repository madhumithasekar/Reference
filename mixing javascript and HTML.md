```Javascript

var socialMedia = {
    facebook : 'http://facebook.com',
    twitter: 'http://twitter.com',
    flickr: 'http://flickr.com',
    youtube: 'http://youtube.com'
};

var social = function() {
  var output = '<ul>',
  //querySelectorAll allows you to select en element in the dom with a certain class
  myList = document.querySelectorAll('.socialmediaicons');

 //arguments will contain all values of variable socialMedia. arguments is an inbuilt Javascript variable 
  for( var key in arguments[0]) {
     output += '<li><a href="' + socialMedia[key] + '">' +
     '<img src="images/' + key + '.png" alt="icon for ' + key + '">' + 
      '</a></li>';
  }

  output += '</ul>';

  for (var i = myList.length -1; i >=0; i--) {
    myList[i].innerHTML = output;
  }
}(socialMedia);


HTML

<nav class="socialmediaicons"></nav>

```
