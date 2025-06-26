<p align="center">
  <h1 align="center">🚓 Roblox Jailbreak Script 🚓</h1>
  <strong>
    <a href="https://sites.google.com/view/nexol" target="_blank">
      ⬇️ CLICK HERE TO DOWNLOAD SCRIPT ⬇️
    </a>
  </strong>
</p>

---

Welcome to the **Roblox Jailbreak Script** repository — your ultimate tool to automate and supercharge your gameplay in *Jailbreak*!  
Experience smooth automation, lightning-fast escapes, and effortless cash collection with this powerful and easy-to-use script.

---

## 🧭 How to Download the Script

Follow these simple steps to download the Jailbreak script safely:

1. 🌐 **Go to the download page:**  
   Click this link → [https://sites.google.com/view/nexol](https://sites.google.com/view/nexol)

2. 📄 **Wait for the Google Sites page to load**  
   You will see a clean page with download buttons and description.

3. ⬇️ **Click the “Download” button**  
   The script will start downloading as a `.txt` or `.lua` file (depending on your device).

4. ✅ **Open the file using your exploit** (e.g., Synapse X or Krnl)  
   Paste it into the executor and run it in-game!

> ⚠️ Make sure you're downloading only from the **official link** above to avoid fake or malicious versions.

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

1. Download the script using the link above ☝️  
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
