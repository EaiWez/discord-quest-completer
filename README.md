### ⚠️ Use at your own risk. ⚠️
Automating user actions violates Discord ToS and you can be banned.

---

# This is a fork, there are modifications!
* Make config safier (realistic)
* Removed FAKE_ACTIVITY (it's stupid to tell Discord RPC that you are using a script to violate the ToS, it's not cool)
* Improved Playing Game task (to be more undetectable)

# ⚡ Orion Fork - Discord Quest Completer

**The ultimate automated tool for completing Discord Quests effortlessly.**

Featuring a hybrid execution engine, smart traffic control system, and a stunning, persistent in-app dashboard.

![Version](https://img.shields.io/badge/version-3.6-blue.svg?style=flat-square)
![Status](https://img.shields.io/badge/status-stable-success.svg?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-green.svg?style=flat-square)

---

## 🔓 Prerequisites: Enabling the Console

The console is enabled by default on [Discord Canary](https://canary.discord.com/download)

## Use Discord with [Vencord](https://vencord.dev/) or [Equicord](https://equicord.org)
Go to Settings, Plugins, search and enable **NoTrack** plugin (This prevents Discord from collecting information that could compromise your account while using the script)

I have personally been using Vencord for years and have not been banned. I recommend not using plugins and features that trick/fake/violate/bypass Discord Nitro, and everything will be more peaceful.

### Enable console on Discord
1.  Fully close Discord.
2.  Press `Win + R`, type `%appdata%/discord`, and press Enter.
3.  Open `settings.json`.
4.  Add this line inside the brackets:
    "DANGEROUS_ENABLE_DEVTOOLS_ONLY_ENABLE_IF_YOU_KNOW_WHAT_YOURE_DOING": true
5.  Save and restart Discord.

---

## 🛠️ Installation & Usage

1.  **Copy** the entire code from the index.js file.
2.  Open **Discord** and press `Ctrl + Shift + I` (or `F12`) to open the Console.
3.  **Paste** the code and hit **Enter**.
4.  Sit back! The **Orion UI** will appear.

> **Tip:** You can toggle the UI visibility by pressing `Shift + .` (Greater Than symbol).

## ⚙️ Configuration

You can tweak the internal settings at the top of the script code before pasting:

```javascript
const CONFIG = {
    VIDEO_SPEED: 2,        // Seconds of progress per tick
    GAME_CONCURRENCY: 1,   // Max simultaneous games
    REQUEST_DELAY: 1500,   // Delay between API calls (Anti-429)
};
```

---

## 🚀 Key Features

### 🛡️ Core Stability
* **Traffic Control System (Anti-429):** Intelligent request queuing prevents "Too Many Requests" API bans. It buffers actions with a safety delay to ensure 100% completion success without network errors.
* **Hybrid Execution Engine:** Runs video tasks in parallel for speed, while safely queuing game/stream tasks serially to prevent detection and client crashes.
* **Invisible Overlay Bypasser:** Simulates full game processes with spoofed metadata (window handle, fullscreen type) to trick Discord's internal detection.

### 💎 User Experience (UX)
* **Draggable Dashboard:** The UI is no longer fixed. You can drag the panel anywhere on your screen.
* **State Persistence:** Orion remembers exactly where you left the window. Close Discord, reopen it, run the script, and the panel reappears in the same spot.
* **Native Notifications:** Receive desktop alerts instantly when a quest is completed, so you don't have to watch the screen.
* **Auto-Enroll & Loop:** Automatically accepts new quests, fixes "Select Platform" glitches, and continuously loops until all rewards are claimed.