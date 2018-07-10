## Working with text fields

```
<input type ="number" id="txt-a-bball" size="3" placeholder="0">
```

//To get the above element in javascript

```
 document.getElementById('txt-a-bball') 
 ```

  returns
```
<input type ="number" id="txt-a-bball" size="3" placeholder="0">
```

//To get the value inside this input box use

```

document.getElementById('txt-a-bball').value 

```

 returns the value inside the textbox

//You can also set the value like this

```

document.getElementById('txt-a-bball').value = 4

```

## Working with forms

//If you want to print all the forms on the page, then use this

```

document.forms[0]  -> prints the first form on the html file

```

returns

```

<form  class="cart" id="cart-hplus" method ="get" action="http://google.com">...</form>

```

//to access all the elements inside the form

```

document.getElementById('cart-hplus').elements

```

returns

```

<input type ="number min="0" id="txt-q-bball" size="3">,
<input type ="number min="0" id="txt-q-bball" size="3">,
<input type ="number min="0" id="txt-q-bball" size="3">,

```

```
document.getElementById('cart-hplus').elements[0] -> will return the first elements

```

returns

```

<input type ="number min="0" id="txt-q-bball" size="3">

```

## How to access dom element which does not have an id but has a name element

eg: 

```
<input type="radio" value="pickup" name="r_method" id="r-method-pickup" checked>

document.getElementById('cart-hplus').r_method

```

returs

```
<input type="radio" value="pickup" name="r_method" id="r-method-pickup checked>,
<input type="radio" value="usps" name="r_method" id="r-method-usps">,
<input type="radio" value=ups" name="r_method" id="r-method-ups">
```
