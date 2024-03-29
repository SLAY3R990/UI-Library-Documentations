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
