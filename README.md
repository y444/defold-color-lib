# Hex Colors Library and Converter for Defold

## How to Start
1. Add https://github.com/y444/defold-color-lib/archive/master.zip as a dependency in your `game.project` file.
2. Fetch library using the main menu: **Project -> Fetch Libraries**.
3. Enable the module adding `local color = require("color-lib.color")` at the beginning of your script.

## How to Use

### Set Color Properties in Hex
Define hex colors using the `set(new_color)` function, where `new_color` is a string formatted as `#00000000`. The module will throw an error if the string is formatted incorrectly.

*Example:* `go.set("#label", "color", color.set("#ff00ff80")) -- sets label's color to purple with 50% opacity`


### Use Predefined Named Colors
The module contains all the named colors as defined [here](https://www.w3schools.com/colors/colors_names.asp). Use them by simply calling them by name.

*Example:* `go.set("#label", "color", color.darkviolet) -- sets label's color to the predefined dark violet color`


### Add Custom Named Colors
You can add your own named colors to use them later in a more convinient way.

Use the `add(new_color_name, new_color)` function, where `new_color_name` is a sting with the name of your new color and `new_color` is a string formatted as `#00000000`. The module will throw an error if the name already exists or the string is formatted incorrectly.

*Example:*

`color.add("half_red","#ff000080") -- defines a new color called half-red`

`go.set("#label", "color", color.half_red) -- sets label's color to the newly defined half-red color`

Uses photos by [Mika Baumeister](https://unsplash.com/@mbaumi?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/paint-container?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
