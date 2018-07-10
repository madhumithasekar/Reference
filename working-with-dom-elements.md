## Working with text fields

```
<input type ="number" id="txt-a-bball" size="3" placeholder="0">
```

//To get the above element in javascript

```javascript
 document.getElementById('txt-a-bball') 
 ```

  returns
```
<input type ="number" id="txt-a-bball" size="3" placeholder="0">
```

//To get the value inside this input box use

```javascript

document.getElementById('txt-a-bball').value 

```

 returns the value inside the textbox

//You can also set the value like this

```javascript

document.getElementById('txt-a-bball').value = 4

```

## Working with forms

//If you want to print all the forms on the page, then use this

```javascript

document.forms[0]  -> prints the first form on the html file

```

returns

```

<form  class="cart" id="cart-hplus" method ="get" action="http://google.com">...</form>

```

//to access all the elements inside the form

```javascript

document.getElementById('cart-hplus').elements

```

returns

```

<input type ="number min="0" id="txt-q-bball" size="3">,
<input type ="number min="0" id="txt-q-bball" size="3">,
<input type ="number min="0" id="txt-q-bball" size="3">,

```

```javascript
document.getElementById('cart-hplus').elements[0] -> will return the first elements

```

returns

```

<input type ="number min="0" id="txt-q-bball" size="3">

```

## How to access dom element which does not have an id but has a name element

eg: 

<input type="radio" value="pickup" name="r_method" id="r-method-pickup" checked>

```javascript

document.getElementById('cart-hplus').r_method

```

returs

```
<input type="radio" value="pickup" name="r_method" id="r-method-pickup checked>,
<input type="radio" value="usps" name="r_method" id="r-method-usps">,
<input type="radio" value=ups" name="r_method" id="r-method-ups">
```

## Working with Select boxes

```
<select id="s-state">
  <option value="volvo">Volvo car</option>
  <option value="saab">Saab car</option>
  <option value="mercedes">Mercedes car</option>
  <option value="audi">Audi car</option>
</select>
```

How to access the value of a select box

```javascript
    
    document.getElementById('s-state').value
 
```

returns the current selected value in select box

returns -> Volvo if selected in the check box

you can also assign values

```javascript
   document.getElementById('s-state').value = "audi"
``` 

If you want to return all the options of a list box you can use the code below

```javascript
   document.getElementById('s-state').options
```

returns

```
  <option value="volvo">Volvo car</option>
  <option value="saab">Saab car</option>
  <option value="mercedes">Mercedes car</option>
  <option value="audi">Audi car</option>
```

If you want to return the selectedIndex of a select box like 1 for volvo, 2 for saab 3 for mercedes, use the code below

```javascript
document.getElementById('s-state').selectedIndex 
```

returns -> 1 if Volvo is selected, returns 2 if saab is selected and so on

You can use options and selectedIndex together if value is not available in certain browsers

```javascript
  
var selectedIdx = document.getElementById('s-state').selectedIndex;
var selectedValue = document.getElementById('s-state').option[selectedIdx].value;

```

### Working with Radio buttons and check boxes

