## Making a third graph

In the this step you are going to start to create your own graph. 

--- task ---

Go to **Choose a Sprite** and select the **Paint** editor.

![Image showing sprite paint tool](images/electricity-paint-editor.png){:width="300px"}

--- /task ---

You may have noticed how the sprites seem invisible. The sprites use the `say`{:class="block3lookss"} block as a title but you cannot see the sprite itself. This is because the sprites are the same colour grey as the backdrop. You now need to create a sprite which is a grey square.

--- task ---

Go to the **Outline** tool and click the square with a red line through it to turn the **Outline** tool off.

![Image showing outline off](images/electricity-paint-editor-outline-off.png){:width="250px"}

--- /task ---

--- task ---

Now add the following values in the **Fill** tool.

Color = 0
Saturation = 0
Brightness = 85

![Image showing grey square values](images/electricity-paint-editor-grey-square.png){:width="250px"}

--- /task ---

--- task ---

Now select the **Rectangle** tool and draw a small square.

![Image showing rectanble took](images/electricity-paint-editor-rectangle-tool.png){:width="250px"}
![Image showing grey rectanble](images/electricity-paint-editor-grey-rectangle.png){:width="400px"}

--- /task ---

Now that your new sprite is a grey square let's give it a name. Below is a table listing a number of countries and the percentage contribution of resources they  use to generate electricity. Choose a country to create a graph for. You could choose any country: one you are from (if it's not already represented), a neighbouring country, somewhere you've visited or what about a country which has uses a lot of one resource?

--- task ---

Investigate the table below and decide on which country you will now create a graph for.

Resource Type | UK | Norway | Indonesia
--- | --- | --- | --- 
**Non-renewables** | 100 | 100 | 100 
**Hydro** | 100 | 100 | 100 
**Marine** | 100 | 100 | 100 
**Geothermal** | 100 | 100 | 100 

--- /task ---

--- task ---

Rename **Sprite1** with the name of the country you have chosen. In this resource, we will refer to this sprite as the **3rd Country** sprite.

![Image showing rename Sprite1](images/electricity-rename-Sprite1.png){:width="300px"}

--- /task ---

When the program is run we want the **3rd Country** spriteto go to a position on the Stage and say its name, just like the **New Zealand** and the **UK** sprites do.

--- task ---

Go to the **Code** editor for the **3rd Country** sprite.

Add the following blocks: `when green flag clicked`{:class="block3events"}, `go to x:` `150`{:class="block3motion"} `y:`{:class="block3motion"} `-140` and a `say`{:class="block3looks"} block where you will type in the name of the country you have chosen.

```blocks3
when green flag clicked
go to x: (150 )y: (-140)
say  () ::looks
```

--- /task ---

--- task ---

Run your program. The sprite should be invisible and it should say its title in the top right-hand side of the Stage.
