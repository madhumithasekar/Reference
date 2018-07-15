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


## Including normalize.css

Normalize.css makes browsers render all elements more consistently and in line with modern standards. Include this file before adding any css file

```
<link rel="stylesheet" type="text/css" href="normalize.css">
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

## Default Styles

/* ---------------------------HTML SECTION --------------------------------- */

```
<head>
  <title></title>
  <link rel="stylesheet" type="text/css" href="grid.css">
  <link rel="stylesheet" type="text/css" href="https://necolas.github.io/normalize.css/8.0.0/normalize.css">
  <link rel="stylesheet" type="text/css" href="style.css">  
</head>

```

/* ----------------------------CSS SECTION ----------------------------------- */

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
 }

 html {
  background-color: #fff;
  color: #555;
  font-family: 'Lato', 'Arial', sans-serif;
  font-weight: 300;
  font-size: 20px;
  text-rendering: optimizeLegibility;  //using this is a good practise
 }
 
 .row {
  max-width: 1140px;
  margin: 0 auto;
}
```

```

/* ----------------------------GRID.CSS ----------------------------------- */

```

/*  SECTIONS  ============================================================================= */

.section {
	clear: both;
	padding: 0px;
	margin: 0px;
}

/*  GROUPING  ============================================================================= */

.row {
    zoom: 1; /* For IE 6/7 (trigger hasLayout) */
}

.row:before,
.row:after {
    content:"";
    display:table;
}
.row:after {
    clear:both;
}

/*  GRID COLUMN SETUP   ==================================================================== */

.col {
	display: block;
	float:left;
	margin: 1% 0 1% 1.6%;
}

.col:first-child { margin-left: 0; } /* all browsers except IE6 and lower */


/*  REMOVE MARGINS AS ALL GO FULL WIDTH AT 480 PIXELS */

@media only screen and (max-width: 480px) {
	.col { 
		/*margin: 1% 0 1% 0%;*/
        margin: 0;
	}
}


/*  GRID OF TWO   ============================================================================= */


.span-2-of-2 {
	width: 100%;
}

.span-1-of-2 {
	width: 49.2%;
}

/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-2-of-2 {
		width: 100%; 
	}
	.span-1-of-2 {
		width: 100%; 
	}
}


/*  GRID OF THREE   ============================================================================= */

	
.span-3-of-3 {
	width: 100%; 
}

.span-2-of-3 {
	width: 66.13%; 
}

.span-1-of-3 {
	width: 32.26%; 
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-3-of-3 {
		width: 100%; 
	}
	.span-2-of-3 {
		width: 100%; 
	}
	.span-1-of-3 {
		width: 100%;
	}
}

/*  GRID OF FOUR   ============================================================================= */

	
.span-4-of-4 {
	width: 100%; 
}

.span-3-of-4 {
	width: 74.6%; 
}

.span-2-of-4 {
	width: 49.2%; 
}

.span-1-of-4 {
	width: 23.8%; 
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-4-of-4 {
		width: 100%; 
	}
	.span-3-of-4 {
		width: 100%; 
	}
	.span-2-of-4 {
		width: 100%; 
	}
	.span-1-of-4 {
		width: 100%; 
	}
}


/*  GRID OF FIVE   ============================================================================= */

	
.span-5-of-5 {
	width: 100%;
}

.span-4-of-5 {
  	width: 79.68%; 
}

.span-3-of-5 {
  	width: 59.36%; 
}

.span-2-of-5 {
  	width: 39.04%;
}

.span-1-of-5 {
  	width: 18.72%;
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-5-of-5 {
		width: 100%; 
	}
	.span-4-of-5 {
		width: 100%; 
	}
	.span-3-of-5 {
		width: 100%; 
	}
	.span-2-of-5 {
		width: 100%; 
	}
	.span-1-of-5 {
		width: 100%; 
	}
}


/*  GRID OF SIX   ============================================================================= */


.span-6-of-6 {
	width: 100%;
}

.span-5-of-6 {
  	width: 83.06%;
}

.span-4-of-6 {
  	width: 66.13%;
}

.span-3-of-6 {
  	width: 49.2%;
}

.span-2-of-6 {
  	width: 32.26%;
}

.span-1-of-6 {
  	width: 15.33%;
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-6-of-6 {
		width: 100%; 
	}
	.span-5-of-6 {
		width: 100%; 
	}
	.span-4-of-6 {
		width: 100%; 
	}
	.span-3-of-6 {
		width: 100%; 
	}
	.span-2-of-6 {
		width: 100%; 
	}
	.span-1-of-6 {
		width: 100%; 
	}
}



/*  GRID OF SEVEN   ============================================================================= */


.span-7-of-7 {
	width: 100%;
}

.span-6-of-7 {
	width: 85.48%;
}

.span-5-of-7 {
  	width: 70.97%;
}

.span-4-of-7 {
  	width: 56.45%;
}

.span-3-of-7 {
  	width: 41.94%;
}

.span-2-of-7 {
  	width: 27.42%;
}

.span-1-of-7 {
  	width: 12.91%;
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-7-of-7 {
		width: 100%; 
	}
	.span-6-of-7 {
		width: 100%; 
	}
	.span-5-of-7 {
		width: 100%; 
	}
	.span-4-of-7 {
		width: 100%; 
	}
	.span-3-of-7 {
		width: 100%; 
	}
	.span-2-of-7 {
		width: 100%; 
	}
	.span-1-of-7 {
		width: 100%; 
	}
}


/*  GRID OF EIGHT   ============================================================================= */

	
.span-8-of-8 {
	width: 100%;
}

.span-7-of-8 {
	width: 87.3%; 
}

.span-6-of-8 {
	width: 74.6%; 
}

.span-5-of-8 {
	width: 61.9%; 
}

.span-4-of-8 {
	width: 49.2%; 
}

.span-3-of-8 {
	width: 36.5%;
}

.span-2-of-8 {
	width: 23.8%; 
}

.span-1-of-8 {
	width: 11.1%; 
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-8-of-8 {
		width: 100%; 
	}
	.span-7-of-8 {
		width: 100%; 
	}
	.span-6-of-8 {
		width: 100%; 
	}
	.span-5-of-8 {
		width: 100%; 
	}
	.span-4-of-8 {
		width: 100%; 
	}
	.span-3-of-8 {
		width: 100%; 
	}
	.span-2-of-8 {
		width: 100%; 
	}
	.span-1-of-8 {
		width: 100%; 
	}
}


/*  GRID OF NINE   ============================================================================= */


.span-9-of-9 {
	width: 100%;
}

.span-8-of-9 {
	width: 88.71%;
}

.span-7-of-9 {
	width: 77.42%; 
}

.span-6-of-9 {
	width: 66.13%; 
}

.span-5-of-9 {
	width: 54.84%; 
}

.span-4-of-9 {
	width: 43.55%; 
}

.span-3-of-9 {
	width: 32.26%;
}

.span-2-of-9 {
	width: 20.97%; 
}

.span-1-of-9 {
	width: 9.68%; 
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-9-of-9 {
		width: 100%; 
	}
	.span-8-of-9 {
		width: 100%; 
	}
	.span-7-of-9 {
		width: 100%; 
	}
	.span-6-of-9 {
		width: 100%; 
	}
	.span-5-of-9 {
		width: 100%; 
	}
	.span-4-of-9 {
		width: 100%; 
	}
	.span-3-of-9 {
		width: 100%; 
	}
	.span-2-of-9 {
		width: 100%; 
	}
	.span-1-of-9 {
		width: 100%; 
	}
}


/*  GRID OF TEN   ============================================================================= */


.span-10-of-10 {
	width: 100%;
}

.span-9-of-10 {
	width: 89.84%;
}

.span-8-of-10 {
	width: 79.68%;
}

.span-7-of-10 {
	width: 69.52%; 
}

.span-6-of-10 {
	width: 59.36%; 
}

.span-5-of-10 {
	width: 49.2%; 
}

.span-4-of-10 {
	width: 39.04%; 
}

.span-3-of-10 {
	width: 28.88%;
}

.span-2-of-10 {
	width: 18.72%; 
}

.span-1-of-10 {
	width: 8.56%; 
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-10-of-10 {
		width: 100%; 
	}
	.span-9-of-10 {
		width: 100%; 
	}
	.span-8-of-10 {
		width: 100%; 
	}
	.span-7-of-10 {
		width: 100%; 
	}
	.span-6-of-10 {
		width: 100%; 
	}
	.span-5-of-10 {
		width: 100%; 
	}
	.span-4-of-10 {
		width: 100%; 
	}
	.span-3-of-10 {
		width: 100%; 
	}
	.span-2-of-10 {
		width: 100%; 
	}
	.span-1-of-10 {
		width: 100%; 
	}
}


/*  GRID OF ELEVEN   ============================================================================= */

.span-11-of-11 {
	width: 100%;
}

.span-10-of-11 {
	width: 90.76%;
}

.span-9-of-11 {
	width: 81.52%;
}

.span-8-of-11 {
	width: 72.29%;
}

.span-7-of-11 {
	width: 63.05%; 
}

.span-6-of-11 {
	width: 53.81%; 
}

.span-5-of-11 {
	width: 44.58%; 
}

.span-4-of-11 {
	width: 35.34%; 
}

.span-3-of-11 {
	width: 26.1%;
}

.span-2-of-11 {
	width: 16.87%; 
}

.span-1-of-11 {
	width: 7.63%; 
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-11-of-11 {
		width: 100%; 
	}
	.span-10-of-11 {
		width: 100%; 
	}
	.span-9-of-11 {
		width: 100%; 
	}
	.span-8-of-11 {
		width: 100%; 
	}
	.span-7-of-11 {
		width: 100%; 
	}
	.span-6-of-11 {
		width: 100%; 
	}
	.span-5-of-11 {
		width: 100%; 
	}
	.span-4-of-11 {
		width: 100%; 
	}
	.span-3-of-11 {
		width: 100%; 
	}
	.span-2-of-11 {
		width: 100%; 
	}
	.span-1-of-11 {
		width: 100%; 
	}
}


/*  GRID OF TWELVE   ============================================================================= */

.span-12-of-12 {
	width: 100%;
}

.span-11-of-12 {
	width: 91.53%;
}

.span-10-of-12 {
	width: 83.06%;
}

.span-9-of-12 {
	width: 74.6%;
}

.span-8-of-12 {
	width: 66.13%;
}

.span-7-of-12 {
	width: 57.66%; 
}

.span-6-of-12 {
	width: 49.2%; 
}

.span-5-of-12 {
	width: 40.73%; 
}

.span-4-of-12 {
	width: 32.26%; 
}

.span-3-of-12 {
	width: 23.8%;
}

.span-2-of-12 {
	width: 15.33%; 
}

.span-1-of-12 {
	width: 6.86%; 
}


/*  GO FULL WIDTH AT LESS THAN 480 PIXELS */

@media only screen and (max-width: 480px) {
	.span-12-of-12 {
		width: 100%; 
	}
	.span-11-of-12 {
		width: 100%; 
	}
	.span-10-of-12 {
		width: 100%; 
	}
	.span-9-of-12 {
		width: 100%; 
	}
	.span-8-of-12 {
		width: 100%; 
	}
	.span-7-of-12 {
		width: 100%; 
	}
	.span-6-of-12 {
		width: 100%; 
	}
	.span-5-of-12 {
		width: 100%; 
	}
	.span-4-of-12 {
		width: 100%; 
	}
	.span-3-of-12 {
		width: 100%; 
	}
	.span-2-of-12 {
		width: 100%; 
	}
	.span-1-of-12 {
		width: 100%; 
	}
}
```
