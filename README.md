# css UI Library
An Advanced UI Library
v1.0.0

# Loadstring:
> To implement the UI, you need this code inside a executor.
```
local Library = loadstring(game:HttpGet("https://github.com/l0ckerV5/Krash/raw/main/Source"))()
```

# Creating the UI:
> To create the ui, you use this code below the previous code, make sure theres spacing for organization.
```
local Window = Library:CreateWindow("Krash UI Library", Vector2.new(300, 300), Enum.KeyCode.RightShift)
```
> you can customize the 'Krash UI Library' part to display whatever is to your liking.

# Creating Tabs:

```
local TestTab = Window:CreateTab("Test")
```

# Creating Sections:

```
local Example = TestTab:CreateSector("Example", "left")
```

# Creating Buttons:

```
Example:AddButton(
    "Button!",
    function()
        print("Button Pressed!")
    end
)
```

# Creating Toggles:

```
Example:AddToggle(
    "Toggle!",
    false,
    function(first)
       Enabled = first
    end
)
```

# Creating Textboxes:

```
Example:AddTextbox(
    "Textbox",
    100,
    function(State)
        Test = State
    end
)
```

# Creating Dropdown:

```
Example:AddDropdown(
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
Example:AddSlider(
    "Slider",
    0,
    50,
    100,
    1,
    function(State)
       
    end
)
```

# Thanks Message
> Thanks for using css UI Library, its a honor to be the UI Designer of a future scripter. If you want to contact me, please send a friend request on discord, my username is l0ckerV5.. Happy Coding!
