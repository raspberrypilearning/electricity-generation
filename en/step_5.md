## Build a pen

In this step, you will learn how to use the `Pen`{:class="block3extensions"} extension blocks to draw on the Stage.

--- task ---

Click on the **Code** tab for your **3rd Country** sprite, and then click the `Pen`{:class="block3extensions"} extension block (in the bottom left-hand corner of the screen).

![png of pen extension block](images/pen-extension.png){:width="400px"}

--- /task ---

Move your pen to the correct starting position.

--- task ---

Underneath your `when green flag clicked`{:class="block3events"} block, insert three `Motion`{:class="block3motion"} blocks: 
+ A `go to x: y:`{:class="block3motion"} block, change the values to `x:`{:class="block3motion"} `120` and `y:`{:class="block3motion"} `-140`. 
+ A `set rotation style`{:class="block3motion"} block, and select `don't rotate`{:class="block3motion"} from the drop-down menu
+ A `point in direction 90`{:class="block3motion"} block.

```blocks3
when flag clicked
+ go to x:(120) y: (-140)
+ set rotation style [don't rotate v]
+ point in direction (90)
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

Prepare the pen and set its size.

--- task ---

Add a `set pen size to 1`{:class="block3extensions"} block, and change the value to `2` so the pen is slightly thicker. Insert a `pen down`{:class="block3extensions"} block to get ready to draw.

```blocks3
when flag clicked
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
+set pen size to (2)
+pen down
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

You need to make sure that the program clears the pen marks from the Stage and lifts the pen up `when green flag clicked`{:class="block3events"}.

--- task ---

Add an `erase all`{:class="block3extensions"} block and a `pen up`{:class="block3extensions"} block at the top of your code, underneath the `when green flag clicked`{:class="block3events"} block.  

```blocks3
when flag clicked
+ erase all
+ pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

The pen colour will change as it draws each resource. In order to compare the resources generated across multiple countries, the colour that represents each resource needs to be the same for each country. After the pen has finished drawing the categories, it will turn to the colour of the backdrop i.e. grey.

--- task ---

Add seven `set pen colour to`{:class="block3extensions"} blocks into your code. These will represent the six categories, plus an additional colour to represent the background.

```blocks3
when flag clicked
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
+ set pen color to []
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

You now need to change the colours of each block to represent the different colours you have chosen for the resources. 

--- task ---

Click on the first `set pen colour to`{:class="block3extensions"} block and select the **Colour picker** tool. Click on the first resource in your key. The circle will then turn to your chosen colour. 

Repeat this for each of the resources in turn, so you don't get the order of the resource colours muddled up. 

Don't forget to use the backdrop colour for the seventh `set pen colour to`{:class="block3extensions"} block, you can get this by hovering anywhere in the background of the Stage.

--- /task ---

Lift the pen when the column has finished drawing.

--- task ---

Add a `pen up`{:class="block3extensions"} block to your code.

```blocks3
when flag clicked
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
set pen color to [#5e6766]
set pen color to [#37e4db]
set pen color to [#e4d748]
set pen color to [#169bb0]
set pen color to [#ab7519]
set pen color to [#00a42c]
set pen color to [#dadada]
+pen up
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

--- task ---

Although the 3rd Country sprite is set up, it doesn’t appear on the graph because you haven't inputted any resource data. You’ll have the chance to input data and check your code in the next step.

--- /task ---

--- save ---
