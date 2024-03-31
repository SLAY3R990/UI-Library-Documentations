# Mobile Kavo UI
This is for the sole purpose of being able to create a GUI easier.

##  Booting the Library

This boots the mobile library.

Put this at the beginning of your code.
 

```lua
local Library = loadstring(game:HttpGet("https://pastebin.com/raw/vff1bQ9F"))()
```

## Creating a Window

This will create the GUI.

```lua
local Window = Library.CreateLib("TITLE", "DarkTheme")
--[[ 
Themes:
LightTheme
DarkTheme
GrapeTheme
BloodTheme
Ocean
Midnight
Sentinel
Synapse
Serpent

String 1: Title of the GUI.
String 2: Color theme for the GUI. 
]]--
```

## Creating a Tab
This will create a tab for your scripts in the GUI.

```lua
local Tab = Window:NewTab("TabName")

--[[
String 1: Name of the tab.
]]--
```

## Creating a Section
This will create a section for your tab. (smaller version of a tab)

```lua
local Section = Tab:NewSection("Section Name")

--[[
String 1: Name of the section.
]]--
```

## Creating a Button
This will create a button that you can make do something when you click it.

```lua
Section:NewButton("ButtonText", "ButtonInfo", function()
    print("Clicked")
end)

--[[
String 1: Name of the button.
String 2: Description of the button.
String 3: Console message when clicked.
Function 1: What the button does (loadstring or code)
]]--
```

## Creating a Label
This creates text in the GUI.

```lua
Section:NewLabel("LabelText")

--[[
String 1: What the label says.
]]--
```

## Creating a Toggle
This creates a switch in the GUI that you can make do something.

```lua
Section:NewToggle("ToggleText", "ToggleInfo", function(state)
    if state then
        print("Toggle On")
    else
        print("Toggle Off")
    end
end)

--[[
String 1: Name of the toggle.
String 2: Description of the toggle.
Function 1: What the toggle does.
String 3: What the console says when it is switched on.
String 4: What the console says when it is switched off.
]]--
```

## Creating a Slider
This will create a slider that you can use to control something.

```lua
Section:NewSlider("SliderText", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
--[[
self explanatory
]]--
```



