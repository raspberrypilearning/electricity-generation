## Draw the column

In this step you are going to use the energy variables for this sprite to draw the stacked column.

In Scratch, you can define your own blocks. This is extremely useful when setting up a series of instructions you want to use in different places throughout your program. 

--- task ---

Go to the My Blocks menu and click on **Make a block**. Set the block name to "draw" and click on **Add an input number or text**. Change the value `number or text` to `amount` then click ok. 

You'll see a new header block has been created in the Code area.

```blocks3
define draw (amount)
```

--- /task ---

Insert a repeat loop to your code to repeat the instructions for the number of times held in `amount`{:class="block3myblocks"}

--- task ---

Add a `repeat`{:class="block3control"} block underneath your new `define`{:class="block3myblocks"} block. Drag an `amount`{:class="block3myblocks"} block from your `define`{:class="block3myblocks"} block into your repeat loop.

![gif of dragging amount](images/drag-amount.gif)

```blocks3
define draw (amount)
+repeat (amount)
end
```

--- /task ---

The column will be created by moving the **3rd Country** sprite 50 steps with the pen down before turning it round 180 degrees then moving up the stage slightly.

--- task ---

Add `Motion`{:class="block3motion"} blocks inside your repeat loop: a `move 50 steps`{:class="block3motion"} block, a `turn right 180 degrees`{:class="block3motion"} block and a `change y by 2`{:class="block3motion"} block.

```blocks3
define draw (amount)
repeat (amount)
+move (50) steps
+turn right (180) degrees
+change y by (2)
end
```

--- /task ---

Create a smooth animation by hiding the **3rd Country** sprite before it draws the column and showing it again once the column is complete.

--- task ---

Add a `hide`{:class="block3looks"} block to the **3rd Country** sprite before it draws the column. Add a `show`{:class="block3looks"} block to make the **3rd Counry** sprite visible at the end of the column build.

```blocks3
when flag clicked
erase all
set (nonrenewable) to (17)
set (wind) to (17)
set (solar) to (17)
set (hydro) to (17)
set (geothermal) to (17)
set (bioenergy) to (15)
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
+hide
set pen color to [#5e6766]
set pen color to [#e4e7e2]
set pen color to [#37e4db]
set pen color to [#e4d748]
set pen color to [#169bb0]
set pen color to [#ab7519]
set pen color to [#00a42c]
set pen color to [#dadada]
pen up
+show
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

Now the draw code is defined we need to insert the newly defined blocks into the `when flag clicked`{:class="block3events"} script. 

--- task ---

From the My Blocks menu insert a `draw`{:class="block3myblocks"} block after each of the `set pen color to`{:class="block3extensions"} blocks. Drag your variables across to the draw blocks in turn in the following order `nonrenewable`{:class="block3variables"}, `wind`{:class="block3variables"}, `solar`{:class="block3variables"}, `hydro`{:class="block3variables"}, `geothermal`{:class="block3variables"}, `bioenergy`{:class="block3variables"}. In the last remaining `draw`{:class="block3myblocks"} block type the value `1`to add a line the same colour as the background to the top of the column.

```blocks3
when flag clicked
erase all
set (nonrenewable) to (17)
set (wind) to (17)
set (solar) to (17)
set (hydro) to (17)
set (geothermal) to (17)
set (bioenergy) to (15)
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
hide
set pen color to [#5e6766]
+draw (nonrenewable)
set pen color to [#e4e7e2]
+draw (wind)
set pen color to [#37e4db]
+draw (tide)
set pen color to [#e4d748]
+draw (solar)
set pen color to [#169bb0]
+draw (hydro)
set pen color to [#ab7519]
+draw (geothermal)
set pen color to [#00a42c]
+draw (bioenergy)
set pen color to [#dadada]
+draw (1)
pen up
show
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

--- task ---

Test your project the column for the **3rd Country** will now complete showing the values you have chosen. When you hover over each category the energy label will show.

--- /task ---
