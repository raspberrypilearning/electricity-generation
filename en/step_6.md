## Draw the third column

In this step you are going to use the resource variables to draw the column for your chosen **3rd Country** sprite.

In Scratch, you can **Make a Block** and add any Scratch blocks into this new script. This is extremely useful when you want to reuse a script elsewhere in your program.

--- task ---

Go to the **My Blocks** menu and click on **Make a Block**. Set the block name to "draw" and click on **Add an input number or text**. Change the value `number or text` to `amount` and then click `ok`. 

You'll see a new **define** block has been created in the **Code** area of the **3rd Country** sprite.

```blocks3
define draw (amount)
```

--- /task ---

The first line in the column will be created by moving the **3rd Country** sprite 50 steps with the pen down before turning it round 180 degrees and then moving up the stage slightly.

--- task ---

Add three `Motion`{:class="block3motion"} blocks: `move 50 steps`{:class="block3motion"} block; `turn right 180 degrees`{:class="block3motion"} block; and `change y by 2`{:class="block3motion"}.

```blocks3
define draw (amount)
+move (50) steps
+turn right (180) degrees
+change y by (2)
```

--- /task ---

Now the draw code is defined we need to insert the newly defined blocks into the `when flag clicked`{:class="block3events"} script. 

--- task ---

From the **My Blocks** menu insert a `draw`{:class="block3myblocks"} block after each of the `set pen color to`{:class="block3extensions"} blocks. Drag your variables across to the draw blocks in turn in the following order:
+ `nonrenewable`{:class="block3variables"}
+ `wind`{:class="block3variables"}
+ `solar`{:class="block3variables"}
+ `hydro`{:class="block3variables"}
+ `geothermal`{:class="block3variables"}
+ `bioenergy`{:class="block3variables"}. 

In the last remaining `draw`{:class="block3myblocks"} block type the value `1`. This will add a line the same colour as the backdrop and appear to clean up the end of the column.

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

Run your program. In the **3rd Country** sprite, you should see the pen draws just one thin line for each resource. In order for the pen to draw the full column you need to repeat the number of lines the pen is instructed to draw so it draws the correct amount for each resource.

--- /task ---

--- task ---

Add a `repeat`{:class="block3control"} block underneath the `define`{:class="block3myblocks"} block. Drag the rounded block `amount`{:class="block3myblocks"} from the `define`{:class="block3myblocks"} block in to the repeat loop.

![gif of dragging amount](images/drag-amount.gif)

```blocks3
define draw (amount)
+repeat (amount)
+move (50) steps
+turn right (180) degrees
+change y by (2)
end
```

--- /task ---

So that the speech bubble only shows at the very end of the drawn column you need to hide the **3rd Country** sprite. The **3rd Country** sprite won't show because it's the same colour as the backdrop but the speech bubble will show unless you hide it until the pen has finished drawing the column. This will create a smooth animation.

--- task ---

Add a `hide`{:class="block3looks"} block to the **3rd Country** sprite before it draws the column. Add a `show`{:class="block3looks"} block to make the **3rd Counry** sprite visible at the end of the drawn column.

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

--- task ---

Test your project. The column for the **3rd Country** will now complete showing the values you have chosen. When you hover over each resource their label will show.

--- /task ---

--- save ---
