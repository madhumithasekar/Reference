## Remove default margins 

All browsers set default margins for HTML elements if we dont specify any. To remove the default margins use the below code

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

## What is box sizing?

![alt text](images/box-sizing.jpg "Box Sizing Images")

---

## Block Elements and Inline Elements

In HTML there are block elements and inline elements

```
<h1> and <p> tags are examples of block elements. 

<img> <a href>, <strong> and <em> are examples of inline elements. 

```

You cannot set height and width for inline elements.

Block elements are stacked vertically one after another.

Inline elements are stacked vertically one aside another. 

![alt text](images/block-inline-elements.jpg "Block and Inline elements")

---

##  Using the container.

Put all the elements inside a container and set the container like this

Steps:

   
   2. Make the container centered 

```
.container {
  Step 1: Set width of the container
   width: 1140px;
  Step 2: Make the DIV centered. auto means that the left and right margin are adjusted automatically according to the context of the           element which is the browser window. So if you adjust the browser window the content stays centered.
   margin-left: auto;  
   margin-right: auto;
}
```
![alt text](images/centeranything-4.jpg "Centering a DIV")

---

## Understanding the float and clearfix property

![alt text](images/float-left-1.png "floating a DIV")

After giving float:left then it would look like this but see the yellow box also has moved to the right side. 

![alt text](images/float-left-2.png "floating a DIV")

To resolve such issue use clearfix property shown below

![alt text](images/float-left-3.png "floating a DIV")

```
  .clearfix:after {
   content: "",
   display: table;
   clear: both;
}

```

---

## Working with Images

When you put an image use the below css. auto is used to maintain the aspect ratio of the image

```
img{
   height: 150px;
   width: auto;
}
```

---
 
## Postion: absolute and position: relative

![alt text](images/position.png "floating a DIV")

``` 	     
.red{
	background-color: red;
	position: relative; //put relative for the parent DIV
}

.blue{
    background-color: blue;
    position: absolute; //put absolute for the child DIV
    top:0;
    right:0;
}
 


     <div class ="red">

            This is red
    
         <div class = "blue" > This is blue</div>
   
     </div>

```

---

## Typography - Fonts and Line Spacing

### Rules:

1. Use a font size of 15px - 25px for body text

2. For headlines you can use a font size of 60px

Note: When you increase the font size always decrease the font weight of the text. This ensures that the text doesn't steal too much attention from the rest of the content and it makes the text look less bulky.

3. For sub-headlines you can use a font size of 32px

4. Use a line spacing of 120% and 150% of the font size. So if the font size is 15px use a line spacing of 15*120% = 18px


### Fonts

1. you can either use sans-serif fonts or serif fonts
  
   some very good sans-serif fonts

  * Open Sans
  * Lato
  * Raleway
  * Monsterrat
  * PT sans

  some very good serif fonts

  * Cardo
  * Merriweather
  * PT Serif

  You can also mix sans-serif fonts for body and serif fonts for heading

---
