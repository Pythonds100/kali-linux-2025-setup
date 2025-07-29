# 🐧 Kali Linux Installation on Android via Termux (2025)

> 💡 Install Kali NetHunter inside Termux and fix XFCE4 panel errors (if any).  
> ⚠️ For **educational use only**. Do not misuse.

---

## 📋 Requirements

- ✅ Termux (Download from [F-Droid](https://f-droid.org))
- ✅ Android 7.0 or above
- ✅ Stable internet connection
- ✅ 5GB+ storage space

---

## 📦 Installation Commands

Copy and paste the following commands into your Termux terminal one by one:

```bash
# Update all packages
apt update && apt upgrade -y

# Setup storage access
termux-setup-storage

# Install wget to download files
pkg install wget -y

# Download Kali NetHunter installation script
wget -O install-nethunter-termux https://offs.ec/2MceZWr

# Make the script executable
chmod +x install-nethunter-termux

# Run the script
./install-nethunter-termux
```

🕒 This may take some time depending on your internet speed.

---

## 🛠️ Error Fix (If GUI not working properly)

Sometimes, XFCE4 GUI panel does not load correctly. Use these commands to reset it:

```bash
# 1. Quit existing XFCE4 panel
xfce4-panel --quit

# 2. Delete corrupted panel configs
rm -rf ~/.config/xfce4/panel

# 3. Remove broken XML config
rm -rf ~/.config/xfce4/xfconf/xfce-perchannel-xml/xfce4-panel.xml

# 4. Restart panel
xfce4-panel &
```

---

## 📱 Follow & Support

- 🔔 YouTube: [Durgesh Exploits](https://youtube.com/@DurgeshExploits)
- 💬 Telegram: [Durgesh Exploits](https://t.me/ExploitsAbout)

---

## 🧑‍💻 License

This script/document is provided under the **MIT License**.  
Feel free to fork, share, and improve with credits.
