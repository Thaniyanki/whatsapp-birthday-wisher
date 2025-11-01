# 🤖 WhatsApp Birthday Wisher Bot

## 📋 Overview
The **WhatsApp Birthday Wisher Bot** automatically manages and runs your WhatsApp automation environment on any **Raspberry Pi (32-bit or 64-bit)**.  
This bot sets up everything needed — folder structure, Python virtual environment, and all required dependencies — in one simple command.

---

## ⚙️ Features
- Works on **any Raspberry Pi** (32-bit or 64-bit)
- Automatically creates proper folder structure  
  ```
  ~/bot/whatsapp birthday wisher/venv
  ```
- Installs all Python and system dependencies
- Downloads the latest bot script from GitHub
- Creates a `report number` file containing the phone number
- Fully automated setup with a single command

---

## 🚀 Quick Install Command

Run this command on your Raspberry Pi terminal:

```bash
curl -sSL https://raw.githubusercontent.com/Thaniyanki/whatsapp-birthday-wisher/main/whtsapp%20birthday%20wisher.sh | bash
```

This command will:
1. Create the folder structure  
   `~/bot/whatsapp birthday wisher/`
2. Install all dependencies inside a Python virtual environment  
3. Download the bot script (`whatsapp birthday wisher.py`)
4. Display instructions to activate and run the bot

---

## 🐍 Running the Bot

After installation, activate the virtual environment and start the bot:

```bash
cd "~/bot/whatsapp birthday wisher"
source venv/bin/activate
python3 "whatsapp birthday wisher.py"
```

---

## 🧩 Installed Dependencies

The script automatically installs the following packages inside your virtual environment:

```
firebase_admin
gspread
selenium
google-auth
google-auth-oauthlib
google-cloud-storage
google-cloud-firestore
psutil
pyautogui
python3-xlib
requests
Pillow
oauth2client
```

and required system packages:
```
python3
python3-venv
python3-pip
git
curl
unzip
```

---

## 📁 Folder Structure After Installation

```
/home/pi/
 └── bot/
     └── whatsapp birthday wisher/
         ├── venv/
         │   ├── bin/
         │   ├── lib/
         │   └── report number
         └── whatsapp birthday wisher.py
```

---

## 🧠 Notes
- The installer automatically deletes and recreates any old `whatsapp birthday wisher` folder for a clean setup.
- The virtual environment is isolated, so it won’t affect system Python packages.
- You can safely re-run the same install command anytime to refresh the setup.

---

## 🧑‍💻 Author
**Thaniyanki**  
GitHub: [@Thaniyanki](https://github.com/Thaniyanki)
