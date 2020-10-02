## Create the resource variables

In this step you are going to create new resource variables for the **3rd Country** sprite. You will then add values to the variables and then use those values to draw the column for the **3rd Country** sprite. You need to use local variables so that updating the value for one sprite will not change it for the others.

First you will create a variable for non-renewable energy.

--- task ---

Create a new variable by clicking on the `Variables`{:class="block3variables"} block menu.

Then click on the **Make a Variable** button.

--- /task ---

You will title the variable `nonrenewable`. 

--- task ---

Title this variable `nonrenewable`.

**Important**: in order to create variables which contain values specific to the **3rd County**, click **For this sprite only**.

Then click **ok**. 

![png of electricity naming variables](images/electricity-naming-variables.png){:width="400px"}

--- task ---


--- /task ---

Create the remaining resource variables.

--- task ---

Create new variables in the same way remembering to select **For this sprite only** for each new variable:
+ `wind`{:class="block3variables"}
+ `solar`{:class="block3variables"}
+ `hydro`{:class="block3variables"}
+ `geothermal`{:class="block3variables"}
+ `bioenergy`{:class="block3variables"}

--- /task ---

Hide the variables from view.

--- task ---

All the new energy variables are listed in the **Variables** menu. They are also automatically shown on the stage but you don't need them shown there for this project.

Click on the tickboxes next to each variable to hide them from view.

![gif of hiding variables](images/hiding-variables.gif)

--- /task ---

You are now going to input the resources data for your chosen country. Below is the table again so you can easily identify the values.

Resource Type | Brazil | Canada | Iceland | India | Ireland | Norway | Singapore | S.Africa | USA |
| --- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
**Non-renewable** | 18 | 34 | 0 | 81 | 64 | 2 | 99 | 94 | 83 |
**Wind** | 9 | 5 | 0 | 5 | 32 | 4 | 0 | 3 | 7 |
**Solar** | 1 | 1 | 0 | 3 | 0 | 0 | 1 | 1 | 2 |
**Hydro** | 63 | 58 | 70 | 11 | 4 | 94 | 0 | 2 | 7 |
**Geothermal** | 0 | 0 | 30 | 0 | 0 | 0 | 0 | 0 | 0 |
**Bioenergy** | 9 | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 1 |

--- task ---

Add in six `set my variable to`{:class="block3variables"} blocks, one for each type of resource. The below code uses example data for the **3rd Country** but you'll input figures for your chosen country.

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

--- task ---

Double-check that the values for the resources all add up to 100.

--- /task ---

--- save ---
