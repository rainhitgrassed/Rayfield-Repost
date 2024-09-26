## Create Window
```lua
local Rayfield = loadstring(game:HttpGet('https://raw.githubusercontent.com/vFishyTurtle/wiihub/main/rayfield'))()local Window = Rayfield:CreateWindow({
   Name = "Shadow.cc Free",
   LoadingTitle = "You Loaded Shadow.cc Free",
   LoadingSubtitle = "by NectoVerse Development on discord.",
   ConfigurationSaving = {
      Enabled = true,
      FolderName = nil, -- Create a custom folder for your hub/game
      FileName = "idk"
   },
   KeySystem = false, -- turned
   KeySettings = {
      Title = "idgaf this is free go lick my balls lil nigger",
      Subtitle = "Skidder? nuh uh",
      Note = "Nuh uh",
      FileName = "No2024only28373", -- nuh uh
      SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
      GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
      Key = {"No2024only2030","Raw808"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
   }
})
```
## Create Tab
```lua
local MainTab = Window:CreateTab ("Home", 4483362458) -- Title, Image
```

## Create Section
```lua
local Section = Tab:CreateSection("Section Example")
```

## Create Toggle
```lua
local Toggle = Tab:CreateToggle({
	Name = "Toggle Example",
	CurrentValue = false,
	Flag = "Toggle1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
	Callback = function(Value)
      
	end,
})
```

## Create Slider
```lua
local Slider = Tab:CreateSlider({
	Name = "Slider Example",
	Range = {0, 100},
	Increment = 10,
	Suffix = "Bananas",
	CurrentValue = 10,
	Flag = "Slider1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
	Callback = function(Value)
      
	end,
})
```

## Create Dropdown
```lua
local Dropdown = Tab:CreateDropdown({
	Name = "Dropdown Example",
	Options = {"Option 1","Option 2"},
	CurrentOption = "Option 1",
	Flag = "Dropdown1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
	Callback = function(Option)
      
	end,
})
```

## Create Keybind
```lua
local Keybind = Tab:CreateKeybind({
	Name = "Keybind Example",
	CurrentKeybind = "Q",
	HoldToInteract = false,
	Flag = "Keybind1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
	Callback = function(Keybind)
      
	end,
})
```
