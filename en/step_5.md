## Create the resource variables

In this step you are going to set energy variables for this sprite only then use those values to draw the stacked column. By making variables unique to individual sprites you can reuse the same names throughout the project but enter different numbers into them for each different country sprite. Updating the value for one sprite will not change it for the others.

Create a variable for non-renewable energy. 

--- task ---

Create a new variable by clicking on the `Variables`{:class="block3variables"} blocks menu.

Then click on the **Make a Variable** button.

You can give your variable a name. Call this variable nonrenewable.

Select **For this sprite only** then click **ok**.

--- /task ---

Create the remaining energy variables.

--- task ---

Create new variables for `wind`{:class="block3variables"}, `tide`{:class="block3variables"}, `solar`{:class="block3variables"}, `hydro`{:class="block3variables"}, `geothermal`{:class="block3variables"} and `bioenergy`{:class="block3variables"} in the same way. 

Make sure to select **For this sprite only**.

--- /task ---

Hide the variables from view.

--- task ---

All the new energy variables are listed in the Variables menu. They are also shown on screen but we don't need to see them. 

Click on the tickboxes next to each variable to hide it from view. 

![gif of hiding variables](images/hiding-variables.gif)

--- /task ---

Set your variables to the energy amounts for your chosen country.

--- task ---

Add in six `set my variable to`{:class="block3variables"} blocks, one for each type of energy. Set the values to be the energy levels for your chosen country, remember to double-check that they all add up to 100.

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

