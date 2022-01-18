-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local main = Instance.new("Frame")
local AnimeVillage = Instance.new("TextButton")
local PirateDocks = Instance.new("TextButton")
local PurpleForest = Instance.new("TextButton")
local Teleport = Instance.new("TextLabel")

--Properties:

ScreenGui.Parent = game.CoreGui
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

main.Name = "main"
main.Parent = ScreenGui
main.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
main.Position = UDim2.new(0.0209854022, 0, 0.277039856, 0)
main.Size = UDim2.new(0, 268, 0, 235)
main.Active = true
main.Draggable = true

AnimeVillage.Name = "Anime Village"
AnimeVillage.Parent = main
AnimeVillage.BackgroundColor3 = Color3.fromRGB(0, 255, 127)
AnimeVillage.Position = UDim2.new(0.0485074632, 0, 0.148936167, 0)
AnimeVillage.Size = UDim2.new(0, 107, 0, 52)
AnimeVillage.Font = Enum.Font.SourceSans
AnimeVillage.Text = "Anime Village"
AnimeVillage.TextColor3 = Color3.fromRGB(0, 0, 0)
AnimeVillage.TextSize = 14.000
AnimeVillage.MouseButton1Down:connect(function()
	local args = {
		[1] = "world",
		[2] = "Anime Village"
	}

	game:GetService("ReplicatedStorage").Remotes.RequestTeleport:InvokeServer(unpack(args))

end)

PirateDocks.Name = "Pirate Docks"
PirateDocks.Parent = main
PirateDocks.BackgroundColor3 = Color3.fromRGB(0, 255, 127)
PirateDocks.Position = UDim2.new(0.0485074632, 0, 0.430950552, 0)
PirateDocks.Size = UDim2.new(0, 107, 0, 52)
PirateDocks.Font = Enum.Font.SourceSans
PirateDocks.Text = "Pirate Docks"
PirateDocks.TextColor3 = Color3.fromRGB(0, 0, 0)
PirateDocks.TextSize = 14.000
PirateDocks.MouseButton1Down:connect(function()
	local args = {
		[1] = "world",
		[2] = "Pirate Docks"
	}

	game:GetService("ReplicatedStorage").Remotes.RequestTeleport:InvokeServer(unpack(args))

end)
PurpleForest.Name = "Purple Forest"
PurpleForest.Parent = main
PurpleForest.BackgroundColor3 = Color3.fromRGB(0, 255, 127)
PurpleForest.Position = UDim2.new(0.0485074632, 0, 0.724475741, 0)
PurpleForest.Size = UDim2.new(0, 107, 0, 52)
PurpleForest.Font = Enum.Font.SourceSans
PurpleForest.Text = "Purple Forest"
PurpleForest.TextColor3 = Color3.fromRGB(0, 0, 0)
PurpleForest.TextSize = 14.000
PurpleForest.MouseButton1Down:connect(function()
	local args = {
		[1] = "world",
		[2] = "Purple Forest"
	}

	game:GetService("ReplicatedStorage").Remotes.RequestTeleport:InvokeServer(unpack(args))

end)
Teleport.Name = "Teleport"
Teleport.Parent = main
Teleport.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Teleport.BorderSizePixel = 0
Teleport.Position = UDim2.new(0.0485074632, 0, 0.0510638282, 0)
Teleport.Size = UDim2.new(0, 107, 0, 23)
Teleport.Font = Enum.Font.SourceSans
Teleport.Text = "Teleport"
Teleport.TextColor3 = Color3.fromRGB(255, 255, 255)
Teleport.TextSize = 14.000
