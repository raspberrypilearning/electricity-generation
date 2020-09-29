## Create the resource variables

In this step you are going to set energy variable for this sprite only then use those values to draw the stacked column.

Set the values of already created variables for each energy category. 

--- task ---

Add in six `set my variable to`{:class="block3variables"} blocks, one for each type of energy. Set the values to be any numbers as long as they all add up to 100.

```blocks3
when flag clicked
erase all
+set (nonrenewable) to (17)
+set (wind) to (17)
+set (solar) to (17)
+set (hydro) to (17)
+set (geothermal) to (17)
+set (bioenergy) to (15)
pen up
go to x:(120) y: (-140)
set rotation style [don't rotate v]
point in direction (90)
set pen size to (2)
pen down
set pen color to [#5e6766]
set pen color to [#e4e7e2]
set pen color to [#37e4db]
set pen color to [#e4d748]
set pen color to [#169bb0]
set pen color to [#ab7519]
set pen color to [#00a42c]
set pen color to [#dadada]
pen up
go to x: (160) y: (70)
say [3rd Country]
```

--- /task ---

