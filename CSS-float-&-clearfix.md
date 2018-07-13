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
