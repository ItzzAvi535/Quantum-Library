# Quantum Library

Loadstring
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/ItzzAvi535/Quantum-Library/refs/heads/main/Library", true))()
```
Create Window:
```lua
local window = library:AddWindow("My Awesome Script", {
    main_color = Color3.fromRGB(255, 0, 0), -- Change ( Theme )
    main_size = Vector2.new(600, 340),
    Key_system = false, -- true to disable key system
    Key = "Avi",
    Note = "Made by Itzzavi." -- your note here
})
```
AddParagraph:
```lua
local Paragraph = Tab:AddParagraph("Hello World")
```

UpdateParagraph:
```lua
Paragraph:SetContent("Updated!")
```

AddLabel:
```lua
Main:AddLabel("This is a test label")
```

AddTab:
```lua
local Main = window:AddTab("Main")
```
AddButton:
```lua
Main:AddButton("Test Button", function()
    -- your code here
end)
```
AddToggle:
```lua
local Toggle = Main:AddToggle("Test Toggle", function(state)
    print("Toggle state:", state)
end)
```
AddTextBox:
```lua
local Textbox = Main:AddTextBox("Test Textbox", function(text)
    print("Text entered:", text)
end)
```
AddDropdown:
```lua
local Dropdown = Main:AddDropdown("Test Dropdown", function(text)
    print("Dropdown selected:", text)
end)
Dropdown:Add("Option1")
Dropdown:Add("Option2")
Dropdown:Add("Option3")
```

AddKeybind:
```lua
local Keybind = Main:AddKeybind("Test Keybind", function(key)
    print("Keybind set to:", key.Name)
end)
```
