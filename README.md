# css UI Library
An Advanced UI Library
v1.0.0

- by l0ckerV5

# Loadstring:
> To implement the UI, you need this code inside a executor.
```
local css = loadstring(game:HttpGet("https://rentry.org/css-source/raw"))()
```

# Creating the UI:
> To create the ui, you use this code below the previous code, make sure theres spacing for organization.
```
local Window = css:CreateWindow("css", Vector2.new(350, 250), Enum.KeyCode.RightShift)
```
> you can customize the 'css' part to display whatever is to your liking.

# Creating Watermark

```
css:CreateWatermark("v1.0.0", "right")
```

# Creating Tabs:

```
local Tab = Window:CreateTab("Tab")
```

# Creating Sections:

```
local Section = Tab:CreateSector("Section", "left")
```

# Creating Buttons:

```
Section:AddButton(
    "Button!",
    function()
        print("Button Pressed!")
    end
)
```

# Creating Toggles:

```
Section:AddToggle(
    "Toggle!",
    false,
    function(first)
       Enabled = first
    end
)
```

# Creating Textboxes:

```
Section:AddTextbox(
    "Textbox",
    100,
    function(State)
        Test = State
    end
)
```

# Creating Dropdown:

```
Section:AddDropdown(
    "Dropdown",
    {"Option1", "Option2", "Option3", "Option4", "Option5"},
    "Option1",
    false,
    function(Option)
        Choice = "Option"
    end
)
```

# Creating Slider:

```
Section:AddSlider(
    "Slider",
    0,
    50,
    100,
    1,
    function(State)
       
    end
)
```

# Creating Config

```
Tab:CreateConfigSystem("left")
```

# Thanks Message
> Thanks for using css UI Library, its a honor to be the UI Designer of a future scripter. If you want to contact me, please send a friend request on discord, my username is l0ckerV5.. Happy Coding!
