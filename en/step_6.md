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

Insert a repeat loop to your code to repeat the instructions for the number of times held in `amount`

--- task ---

Add a repeat block underneath your new define block. Drag an `amount` block from your define block into your repeat loop.

![gif of dragging amount](images/drag-amount.gif)

```blocks3
define draw (amount)
+repeat (amount)
end
```

--- /task ---

The column will be created by moving the **3rd Country** sprite 50 steps with the pen down before turning it round 180 degrees then moving up the stage slightly.

--- task ---

Add Motion blocks inside your repeat loop: a `move 50 steps` block, a `turn right 180 degrees` block and a `change y by 2` block.

```blocks3
define draw (amount)
repeat (amount)
+move (50) steps
+turn right (180) degrees
+change y by (2)
end
```

--- /task ---

Now the draw code is defined we need to insert the newly defined blocks into the `when flag clicked` script. To create a smooth animation add a `hide` block to the **3rd Country** sprite before it draws the column. To position your column header in the right place add a `show` block to make the **3rd Counry** sprite visible at the end.

--- task ---

hide and show

--- /task ---

--- task ---

draw categories


--- /task ---

--- task ---

draw 1

--- /task ---

--- task ---

test

--- /task ---
