# css UI Library
An Advanced UI Library
v1.0.0
- by l0ckerV5

# Loadstring:
> To implement the UI, you need this code inside a executor.
```
local Library = loadstring(game:HttpGet("https://github.com/l0ckerV5/css/raw/refs/heads/main/Source"))()
```

# Creating the UI:
> To create the ui, you use this code below the previous code, make sure theres spacing for organization.
```
local Window = Library:CreateWindow("css", Vector2.new(350, 250), Enum.KeyCode.RightShift)
```
> you can customize the 'css' part to display whatever is to your liking.

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

# Creating ColorToggle w/ ColorPicker

```
local ColorToggle = 
Section:AddToggle(
    "ColorPicker w/Toggle",
    false,
    function(e)

    end
)
```

```
ColorToggle:AddColorpicker(
    Color3.fromRGB(75, 0,130),
    function(ztx)
   
    end
)
```

# Creating ToggleBind

```
local ToggleBind = 
Section:AddToggle(
    "Keybind w/Toggle",
    false,
    function(e)

    end
)
```

```
ToggleBind:AddKeybind()
```

# Creating Config

```
Tab:CreateConfigSystem("left")
```

# Creating Watermark

```
css:CreateWatermark("v1.0.0", "right")
```

# Thanks Message
> Thanks for using css UI Library, its a honor to be the UI Designer of a future scripter. If you want to contact me, please send a friend request on discord, my username is l0ckerV5.. Happy Coding!
