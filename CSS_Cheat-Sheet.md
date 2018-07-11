### Remove default margins 

All browsers set default margins for HTML elements if we dont specify any. To remove the default margins use the below code

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
```

### What is box sizing?

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

###  Using the container.

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

### Understanding the float and clearfix property

![alt text](images/float-left-1.png "floating a DIV")

After giving float:left then it would look like this but see the yellow box also has moved to the right side. 

![alt text](images/float-left-2.png "floating a DIV")

To resolve such issue use clearfix property shown below

![alt text](images/float-left-2.png "floating a DIV")

```
  .clearfix:after {
   content: "",
   display: table;
   clear: both;
}

```

---



