## Build a pen

In this step, you will learn how to use the `Pen`{:class="block3extensions"} extension blocks to draw on the Stage.

--- task ---

Click on the **Code** tab for your **3rd Country** sprite, and then click the **Add Extension** button in the bottom left-hand corner of the screen.

Select the `Pen`{:class="block3extensions"} extension.

![gif of adding the pen extension](images/pen-extension.gif)

--- /task ---

Move your pen to the correct starting position.

--- task ---

Underneath your `when flag clicked`{:class="block3events"} block add three `Motion`{:class="block3motion"} blocks. Add a `go to x: y:`{:class="block3motion"} block and change the values to x: `120` and y: `-140`. Add a `set rotation style`{:class="block3motion"} block, selecting `don't rotate` from the drop down, and a `point in direction 90`{:class="block3motion"} block.

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

Add a `set pen size to 1`{:class="block3extensions"} block changing the value to `2` so the pen is slightly thicker. Insert a `pen down`{:class="block3extensions"} block to get ready to draw.

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

At the moment you haven't entered any data for the **3rd country** sprite but you can still test that the pen works using the default colour.

--- task ---

Run your project. The pen will draw a line as the **3rd Country** sprite moves into place.

![image of starting line](images/starting-line.png)

--- /task ---

You need to make sure that the program clears the pen marks from the stage and lifts the pen up `when flag clicked`{:class="block3events"}.

--- task ---

Add an `erase all`{:class="block3extensions"} block and a `pen up`{:class="block3extensions"} block at the top of your code underneath `when flag clicked`{:class="block3events"}

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

The pen colour will change as it draws each resource. In order to compare the resources generated across multiple countries, the colour representing each resource needs to match. After the pen has finished drawing the categories it will turn to the colour of the background.

--- task ---

Add seven `set pen colour to`{:class="block3extensions"} blocks into your code. These will represent the six categories plus an additional colour to represent the background.

Change the colours of each block in turn to represent a different colour, the values are in the table below and you can look back to making the grey square on the previous step if you need a reminder about how to change them.

![image of colour chart](images/colour-chart.png)

```blocks3
when flag clicked
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
+ set pen color to [#5e6766]
+ set pen color to [#37e4db]
+ set pen color to [#e4d748]
+ set pen color to [#169bb0]
+ set pen color to [#ab7519]
+ set pen color to [#00a42c]
+ set pen color to [#dadada]
go to x: (160) y: (70)
say [3rd Country]
```

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

Test your project by clicking on the green flag. Though the **3rd Country** sprite is set up it doesn't draw a graph as you haven't inputted any resource data yet.

--- /task ---

--- save ---
