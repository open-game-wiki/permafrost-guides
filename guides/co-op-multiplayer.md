---
title: "Co-op Multiplayer Guide: How to Host, Join, and Fix Connection Issues"
description: "Everything you need to know about 4-player online co-op in Permafrost. Server setup, squad task division, shared shelters, and multiplayer troubleshooting."
category: "Multiplayer"
badge: "VERIFIED IN-GAME DATA • EA 2026"
readingTime: "6 min read"
publishDate: "2026-10-09"
icon: "coop"
lang: "en"
---

*Permafrost* supports full online cooperative multiplayer for up to **4 players** (you and up to three teammates). While braving the arctic wasteland alone is intensely atmospheric, teaming up allows squads to divide labor, construct fortified outposts, and overwhelm dangerous wolf packs.

This guide outlines how to host a server, invite friends, and resolve common Early Access connection hurdles.

---

## 1. How to Host & Join a Co-op Session

Early Access relies on a peer-to-peer hosted server model. Currently, there are no official persistent dedicated servers; the host player holds the world save file:

### Hosting a Game:
1. From the Main Menu, click **Multiplayer**.
2. Select **Host Game** -> Choose an existing world save or create a New World.
3. Configure your server settings:
   * **Server Name:** Set a custom session name.
   * **Max Players:** Default 4.
   * **Privacy:** Set to **Friends Only** or **Password Protected** to prevent random walk-ins from griefing your base.
4. Click **Start Session**. Once loaded into the world, open the Steam Overlay (`Shift + Tab`) to directly invite friends from your friends list.

### Joining a Friend:
* **Via Steam Invite:** Accept your friend's game invite in Steam chat to connect directly.
* **Via In-Game Server Browser:** Click **Multiplayer** -> **Find Game** -> Filter by Server Name and enter the host's password.

---

## 2. Squad Division of Labor (The Ideal 4-Player Meta)

Because resource consumption (food, drinking water, warm shelter) scales with squad size, uncoordinated teams often freeze or starve quickly. Assign these roles:

| Squad Role | Recommended Build | Primary Responsibilities |
| :--- | :--- | :--- |
| **Outpost Architect** | Survivor + Engineer | Tree felling, shelter wall alignment, maintaining the hearth fire |
| **Master Hunter** | Survivor + Tracker | Crafting bows, hunting deer/wolves, curing hides on the Tanning Rack |
| **Deep Miner** | Smuggler + Engineer | Flint, Copper, and Iron extraction from hazardous mountain caves |
| **Combat Scout** | Smuggler + Scavenger | Raiding Solar Farm and ruins for military blueprints, scrap, and firearms |

---

## 3. Common Multiplayer Issues & Fixes

### A. Connection Timed Out / Failed to Join Host
* **Fix 1: Check Steam Status:** Both host and client must have Steam active and running the exact same game patch version.
* **Fix 2: NAT Type & Firewall:** Ensure `Permafrost.exe` has full inbound/outbound permissions through Windows Defender Firewall.
* **Fix 3: Disable Windows Smart App Control:** Some players report that Windows Smart App Control falsely intercepts p2p lobby handshakes. Adding an exclusion resolves the timeout.

### B. Desync & Inventory Duplication
* **Rule for the Host:** Always ensure all players sleep in their respective cots before the host exits to the main menu. Abrupt host disconnects can cause client inventory rollbacks.
