-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local KeySystem = Instance.new("Frame")
local TextLabel = Instance.new("TextLabel")
local Success = Instance.new("TextButton")
local KeyText = Instance.new("TextBox")
local REMOVE = Instance.new("TextButton")
local GetKey = Instance.new("TextButton")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

KeySystem.Name = "Key System"
KeySystem.Parent = ScreenGui
KeySystem.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
KeySystem.BorderColor3 = Color3.fromRGB(0, 0, 0)
KeySystem.Position = UDim2.new(0.267326742, 0, 0.234432235, 0)
KeySystem.Size = UDim2.new(0, 528, 0, 275)
KeySystem.Active = true
KeySystem.Draggable = true

TextLabel.Parent = KeySystem
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.BackgroundTransparency = 1.000
TextLabel.Position = UDim2.new(0.310606033, 0, 0.123636365, 0)
TextLabel.Size = UDim2.new(0, 200, 0, 50)
TextLabel.Font = Enum.Font.SourceSans
TextLabel.Text = "Put key "
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextSize = 30.000

Success.Name = "Success"
Success.Parent = KeySystem
Success.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
Success.BorderColor3 = Color3.fromRGB(30, 30, 30)
Success.Position = UDim2.new(0.310606062, 0, 0.538181782, 0)
Success.Size = UDim2.new(0, 200, 0, 29)
Success.Font = Enum.Font.SourceSans
Success.Text = "Succes"
Success.TextColor3 = Color3.fromRGB(85, 255, 0)
Success.TextSize = 30.000
Success.TextStrokeColor3 = Color3.fromRGB(255, 0, 0)
Success.MouseButton1Click:connect(function()
if string.find(KeyText.Text,"AEAARARARAFSGAG2YYDSUUNSAD9ADADKAKDKADA9DA8DADKADADADASFX") then

		repeat wait() until game.Players.LocalPlayer.Character
		url = "https://raw.githubusercontent.com/xennyy/Xenny-Ware/main/loader.lua"
		loadstring(game:HttpGet(url))()
		game.StarterGui:SetCore("SendNotification",{
			Title = "Key System";
			Text = "Thanks For Using The Script";
			Duration = 10
		})
		KeySystem:Destroy()
elseif string.find(KeyText.Text, "TY9J992U3I12WIMSOAPPAPPAPA00A9A9AS9DIAMMMALAALOAIWUUS") then
	game.StarterGui:SetCore("SendNotification",{
		Title = "Key System";
		Text = "Key Updated";
		Duration = 10
	})
	
else
	game.StarterGui:SetCore("SendNotification",{
		Title = "Key System";
		Text = "Invalid Key ";
		Duration = 10
	})
end
end)
KeyText.Name = "KeyText"
KeyText.Parent = KeySystem
KeyText.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
KeyText.Position = UDim2.new(0.0833333358, 0, 0.389090896, 0)
KeyText.Size = UDim2.new(0, 439, 0, 25)
KeyText.Font = Enum.Font.SourceSans
KeyText.PlaceholderColor3 = Color3.fromRGB(0, 0, 0)
KeyText.PlaceholderText = "Key Here"
KeyText.Text = ""
KeyText.TextColor3 = Color3.fromRGB(0, 0, 0)
KeyText.TextSize = 14.000

REMOVE.Name = "REMOVE"
REMOVE.Parent = KeySystem
REMOVE.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
REMOVE.BorderColor3 = Color3.fromRGB(30, 30, 30)
REMOVE.Position = UDim2.new(0.308712125, 0, 0.712727308, 0)
REMOVE.Size = UDim2.new(0, 200, 0, 25)
REMOVE.Font = Enum.Font.SourceSans
REMOVE.Text = "NeverMind!"
REMOVE.TextColor3 = Color3.fromRGB(255, 0, 0)
REMOVE.TextSize = 30.000
REMOVE.TextStrokeColor3 = Color3.fromRGB(255, 0, 0)
REMOVE.MouseButton1Click:connect(function()
	KeySystem:Destroy()
end)


GetKey.Name = "Get Key"
GetKey.Parent = game.StarterGui.ScreenGui.Key 
GetKey.BackgroundColor3 = Color3.fromRGB(30, 30, 30)
GetKey.BorderColor3 = Color3.fromRGB(30, 30, 30)
GetKey.Position = UDim2.new(0.308712125, 0, 0.836363673, 0)
GetKey.Size = UDim2.new(0, 200, 0, 25)
GetKey.Font = Enum.Font.SourceSans
GetKey.Text = "Get Key"
GetKey.TextColor3 = Color3.fromRGB(255, 255, 0)
GetKey.TextSize = 30.000
GetKey.TextStrokeColor3 = Color3.fromRGB(255, 0, 0)
GetKey.MouseButton1Click(function()
	setclipboard("https://direct-link.net/131909/Key")
	game.StarterGui:SetCore("SendNotification",{
		Title = "Key System";
		Text = "Copied Key Link Go To Chrome And Go To Link And Complete Only 2 Missions";
		Duration = 10
	})
end)

