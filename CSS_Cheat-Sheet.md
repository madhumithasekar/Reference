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

1. You can either use sans-serif fonts or serif fonts
  
   **Some very good sans-serif fonts**

  * Open Sans
  * Lato
  * Raleway
  * Monsterrat
  * PT sans

  **Some very good serif fonts**

  * Cardo
  * Merriweather
  * PT Serif

  You can also mix sans-serif fonts for body and serif fonts for heading

---

## Color combination in Web Design

To choose a color for your website first go to the website below

https://flatuicolors.com and choose any base color

then go the below website

http://www.0to255.com and enter the base color. The above website will create various variations of the base color. Choose any of the five variation and create a color palette to use in your website.

For background colors and text colors, use grey colors

### Mix and match Colors:

If you want to mix and match different base colors then you can use the tool below. It will recommend different colors which will look nice

For information on how to use the color wheel you can check the below YouTube video

https://color.adobe.com/create/color-wheel/

<a href="http://www.youtube.com/watch?feature=player_embedded&v=fuF3foDjHwc" target="_blank"><img src="http://img.youtube.com/vi/fuF3foDjHwc/0.jpg" alt="Adobe Color Wheel" width="560" height="315" border="10" /></a>

They also have a set of color schmes i.e a set of color sets which are to be used in combination. Find the link below

https://color.adobe.com/explore/?filter=most-popular&time=month 

Note: 
  
   * Use the main color to draw attention to your   website like "Call to action button" or any other important element of your website

   * Use the second and third color to compliment the main color

   * Never use black in your design
   
 ---
 
 ## Putting text over images

If you put text directly on an image it will only look good if the image is dark and text is white. 

There are few techniques for making the image and text look good.

1. Overlay the image with a color. The most easiest to use is a black overlay on the top of image and then write text on it. Apart from black you can also use various other color gradients.

2. The second option is to blur the image and the text is shown on the blurred image part on all screen resolutions

3. The third option is to use a technique called "Floor fade technique". Here the image subtly fades towards black at the bottom and white text written over it.

4. Simply putting text on a box like the image shown below. The box should be opaque so that you can still see the image beneath it. In the below case a white color with some transperancy is used. 

![alt text](images/images-box.png "image-box")

---
 
## Including normalize.css

Normalize.css makes browsers render all elements more consistently and in line with modern standards. Include this file before adding any css file

```
<link rel="stylesheet" type="text/css" href="normalize.css">
```

---

## Including Web fonts

  #### Check the Fonts section to find what fonts to use

Link to download fonts: http://google.com/fonts

Quick Introduction on how to use Google fonts. Check the below video

[![Using Google Fonts](http://img.youtube.com/vi/67AbASjp0co/0.jpg)](http://www.youtube.com/watch?v=67AbASjp0co)

You can always set the default font like this

```
html {
font-family: 'Lato', 'Arial', sans-serif;
font-weight: 300;
font-size: 20px;
text-rendering: optimizeLegibility;  //using this is a good practise
}

```

---

## Fluid Grid

We will be using fluid grid to develop our website. The fluid grid that we would be using is 

http://www.responsivegridsystem.com/

Inlcude the above grid.css after normalize.css

```
<link rel="stylesheet" type="text/css" href="grid.css">
```

Note: The downloaded file will have seperate file as 2cols.css, 3cols.css. Combine everything into one and rename it as grid.css and include it here

Using this grid all our content will be in columns. You can have from 1 column in a row to 12 columns in a row.

When using this grid we will be using only one value in px and rest we would be using in percentages

```
 .row{
 	max-width: 1140px;
 	margin-left: auto;
 	margin-right: auto;
 }

```

---

## Elements in HTML

![HTML Elements](images/img_sem_elements.gif "image-box")

  ```
  <article>        
     <aside>                       
     <details>                   
     <figcaption>                 
     <figure>                     
     <footer>                     
     <header>                     
     <main>                       
     <mark>                       
     <nav>                       
     <section>                    
     <summary>                    
     <time>
   
   ```   
---

## Building the header part

  ### Final output:

  We will be creating the below output.

  * Placing image in the header section
  * Placing main text on the image
  * Placing 2 buttons on the image
  * Placing navigation on the image 

  ### Result:
  
  ![Final Result](images/header-final.png "Final Result")
  
  ### STEP 1: ```<header>``` tag

 We will put everything inside ```<header>``` DIV

```
<header> 

</header>
```


### STEP 2: Container

 Now we will create a container inside the ```<header>``` tag

```
<header>

  <div class="hero-text-box">
  	
  </div>

</header>
```

### STEP 3: H1 tag

 Now we will put ```<h1>``` inside the container

```
<header>
	
	<div class="hero-text-box">
       
          <h1>Goodbye junk food. Hello super healthy meals.</h1>
 
	</div>

</header>
```

### STEP 4: BUTTONS

 Now we need two buttons inside the container. For buttons we will use ```<a href>``` tag

```
 <header>	
   <div class="hero-text-box">       
       <h1>Goodbye junk food. Hello super healthy meals.</h1>
       <a href="#">I'm hungry</a> 
       <a href="#">Show me more</a>
   </div>

</header>
```

Result: 

![Result One](images/result-one.png "Result One")  

### STEP 5: Add default styles

  * Add *{}, html{} default for all CSS

```
 * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
 }
``` 

```
 html {
 	background-color: #fff;
 	color: #555;
	font-family: 'Lato', 'Arial', sans-serif;
	font-weight: 300;
	font-size: 20px;
	text-rendering: optimizeLegibility;  //using this is a good practise
 }
```

### STEP 6: background-image

```
header{
	background-image: url(hero.jpg);
}
```

### STEP 7: Image Height

When you set a background image the image only fills the part which has some content like shown below

![Image Scale](images/image-scale.png "Image Scale")

To scale the image to whole view port

```
header{
	background-image: url(hero.jpg);
	height: 100vh; //means 100% of the view port
}
```

Now the image would have scaled like this

![View Port](images/viewport.png "View Port")

### STEP 8: image background-size

Even now if you see the image would be like zoomed in and part of the image will not be visible. See the image below

![View Port](images/viewport.png "View Port")

So resolve this we will have to give background-size

```
header{
	background-image: url(hero.jpg);
	background-size:cover;
	height: 100vh; //means 100% of the view port
}
```
### STEP 9: background-centered

Then you will have to make background centered

```
header{
	background-image: url(hero.jpg);
	background-size:cover;
	background-position: center;
	height: 100vh; //means 100% of the view port
}

```

Now the image will look like this

![Image Cover](images/image-cover.png "Image Cover")

So now even if you resize the browser window the whole image would scale down and be properly shown in the screen.

### Working with Text on images

Now lets see how to place text on images properly

```
 <header>
	
	<div class="hero-text-box">
       
       <h1>Goodbye junk food. Hello super healthy meals.</h1>
       <a href="#">I'm hungry</a> 
       <a href="#">Show me more</a>
	</div>

</header>
```

Always give width for the textbox. 
Then if you want to move the textbox DIV give ```position:absolute``` along with ```top:0``` or ```left:0``` or ```right:0``` or ```bottom:0```

It is also a good practise to give ```transform: translate(-50%, -50%)``` along with ```position:absolute``` and ```top/left/right/bottom```. ```transform:translate``` has better performance than using ```top/left/right/bottom```

```
.hero-text-box {
   position: absolute;
   width: 1140px;
   top:50%;
   left:50%;
   transform: translate(-50%, -50%);
}

```

Now the text would be nicely centered and it will look like this.

![Image Text](images/text.png "Image Text")

### Setting Contrast 

Now if you see the above image text on the image does not look good. As mentioned in the earlier chapter to make text look good on images one way is to put a black transparent background on the image and put a white color text on it.

 #### Adding gradient:

Now we have already learned from the earlier chapter image on text will look good only if the image is transparent or out-of-focus etc and text should be white. So now lets add a transparent overlay on top of the image like this.

```
header{
	background-image: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url(hero.jpg);
	background-size:cover;
	background-position: center;
	height: 100vh; //means 100% of the view port
}
```

Now this will look like this

![Image Cover](images/transparent-image.png "Image Cover")

  #### Making changes to the font
  
   ```
      h1{
          color: #fff;
	  font-size: 200%  // Refer what are good font sizes for heading in the earlier chapters.
      }
   
   ```

   #### So how 200%?
   
    In responsive design eveything should be mentioned in percentages and only in the global scope we should mention pixels. So the global scope is the below code
    
    ```
     html {
 	background-color: #fff;
 	color: #555;
	font-family: 'Lato', 'Arial', sans-serif;
	font-weight: 300;
	font-size: 20px;
	text-rendering: optimizeLegibility;  //using this is a good practise
     }
    
    ```
    
    So when you say font-size:200% it refers to 200% of font-size:20px
    
  #### Decrease the font weight
  
Now remember as in the earlier chapters when the font-size is big decrease the font-weight. Usually ```<h1>``` tag comes with bold formatting.
   
  ```
      h1{
          color: #fff;
	  font-size: 200%  // Refer what are good font sizes for heading in the earlier chapters.
	  font-weight: 300;
      }
   
  ```
   
   Other things that you can do to make ```<h1>``` look better
   
     ```
      h1{
          color: #fff;
	  font-size: 200%  // Refer what are good font sizes for heading in the earlier chapters.
	  font-weight: 300;
	  text-transform: uppercase;
	  letter-spacing: 1px;  // so the letters don't look very compressed
	  word-spacing: 3px; //letters between words
      }
   
  ```
  
   ### Designing the buttons

Now to design the buttons let us add a css class like this. You can also copy and paste the below code if required. All buttons are designed more or less the same way.

 ```
 <header>	
   <div class="hero-text-box">       
       <h1>Goodbye junk food. Hello super healthy meals.</h1>
       <a class="btn btn-full" href="#">I'm hungry</a> 
       <a class="btn btn-ghost" href="#">Show me more</a>
   </div>

</header>
```

//this is the common button style for any buttons

Note: Link is the default state so hence we are changing .btn to .btn:link

```
.btn:link {
   display: inline-block;
   padding: 10px 30px;
   font-weight: 300px;
   text-decoration: none; //this is used to remove underline from <a> tag
   border-radius: 200px; // to get a curved button on all borders
   
}
```

```
.btn-full{
	background-color: #e67e22; //get the color code from flatuicolors.com
	border: 1px solid #e67e22;
	color: #fff -> // to change the text color on the button to white
}
```

```  
.btn-ghost{
   border: 1px solid #e67e22;
   color: #e67e22;
}

```

Every button has four states also called as pseudo states. They are as follows

* Link - Link is the default state
* Visited
* active - When we click on a button
* hover - When we put mouse on a button

 ### Link and Visited:

Here both link and visited has the same style. So you can use the below code

  #### Writing for link and visited

```
.btn:link,
.btn:visited {
   display: inline-block;
   padding: 10px 30px;
   font-weight: 300px;
   text-decoration: none; //this is used to remove underline from <a> tag
   border-radius: 200px; // to get a curved button on all borders
   transition: background-color 0.2s, border 0.2s, color 0.2s // this will create an animation effect to the button and change the background-color, border and font-color slowly
}
```


```
.btn-full:link,
.btn-full:visited{
	background-color: #e67e22; //get the color code from flatuicolors.com
	border: 1px solid #e67e22;
	color: #fff -> // to change the text color or font color on the button to white
	margin-right: 15px;
}
```

```  
.btn-ghost:link,
.btn-ghost:visited{
   border: 1px solid #e67e22;
   color: #e67e22; // to change the text color or font color
}

```

 #### Writing for hover and active

```
.btn:hover,
.btn:active {
	background-color: #cf6d17; //get a darker shade of original button color. Use the 0-255 color tool here
}

```

```
.btn-full:hover,
.btn-full:active{
	border: 1px solid #e67e22;
}
```

```  
.btn-ghost:hover,
.btn-ghost:active{
   border: 1px solid #e67e22;
   color: #fff; // to change the text color or font color
}

```

#### What are block level elements and Inline elements?

```<h1>``` is a block level element by default
```<span>, <a>``` etc. is a inline level element.

Now lets take this ```<h1>``` tag

```<h1>This is a simple text</h1>```

The above ```<h1>``` tag is a block level element and it will take full width of the browser or parent DIV.

Now if you make it like this

```<h1>This is a <span>simple<span> text</h1>```

and if you write the CSS as

```
span{
	display: block;
}
```

The above text would be printed like this

This is a - Line 1
Simple - Line 2
text - Line 3

Now ```<span> simple </span>``` is a block level element and it will take full width of the parent DIV thus takes the next line and "text" is moved to the third line.

Inline element do not take full width rather it takes only the corresponding text width.

For a block level element you can mention width and height as well as margin and padding, left, right, top and bottom.

Inline elements by default do not take any sort of width and you cannot assign them a width like shown below

```
span{
	width: 100% -> this is wrong and nothing will happen here
}
```

Inline elements also cannot have height, margin, top, bottom or padding.

So for an inline element if you want to set padding and margin, set it as inline-block.

eg:

```
span{
	display: inline-block; // not you can set margin, padding etc
}
```

It also dosen't force a line break since all block level elements will force a line break since it takes full width.
   
