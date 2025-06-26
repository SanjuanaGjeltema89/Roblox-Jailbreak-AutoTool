# 🚓 Roblox Jailbreak Script

A powerful and easy-to-use script for [Roblox Jailbreak](https://www.roblox.com/games/606849621/Jailbreak).  
Includes auto arrest, teleportation, and basic automation features.

> ⚠️ For educational purposes only. Use at your own risk.

## 💻 Features

- 👮 Auto Arrest Criminals
- 🚗 Teleport to Player
- 📦 Simple & Lightweight

## 📜 How to Use

1. Copy the code from `script.lua`
2. Open your Roblox Executor (Synapse X, Fluxus, KRNL, etc.)
3. Paste the script and execute in Jailbreak

## 🔧 Example Code

```lua
-- Auto Arrest Script for Roblox Jailbreak
for _, player in pairs(game.Players:GetPlayers()) do
    if player.Team == "Criminals" and player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = player.Character.HumanoidRootPart.CFrame
        wait(0.5)
        local arrestButton = workspace:FindFirstChild("ArrestButton")
        if arrestButton and arrestButton:FindFirstChild("ClickDetector") then
            fireclickdetector(arrestButton.ClickDetector)
        end
    end
end

