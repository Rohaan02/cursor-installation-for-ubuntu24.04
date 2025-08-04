# 🖥️ Install Cursor AI IDE on Ubuntu 24.04

_by Rohaan02 (rohaannadeem2@gmail.com)_

This repository contains an installer script to run **Cursor AI IDE** on Ubuntu 24.04 using an AppImage-based setup.

---

## 📦 Features

- Installs the latest version of Cursor AI IDE
- Automatically handles dependencies (e.g., `figlet`)
- Extracts AppImage and deploys it to `/opt/Cursor`
- Adds a desktop entry for launching from the menu

---

## 📋 Prerequisites

- Ubuntu 24.04
- `git` and `curl` installed
- Internet connection

---

## 🛠️ Installation Steps

1. **Clone the repository**

   ```bash
   git clone --branch Cursor-ubuntu24.04 https://github.com/hieutt192/Cursor-ubuntu.git
   cd Cursor-ubuntu
   ```

2. **Check available files**

   ```bash
   ls
   ```

   Expected output:

   ```
   images  manage_cursor.sh  README.md
   ```

3. **Make the script executable**

   ```bash
   chmod +x manage_cursor.sh
   ```

4. **Run the installer**

   ```bash
   ./manage_cursor.sh install
   ```

   - If `figlet` is not installed, it will be installed automatically.
   - You will see a menu:
     ```
     💿 1. Install Cursor
     🆙 2. Update Cursor
     Please choose an option (1 or 2):
     ```

5. **Choose installation option**

   ```
   1
   ```

   ```bash

   ```

6. **💿 Installing Cursor AI IDE on Ubuntu...**
   How do you want to provide the Cursor AppImage?
   📥 1. Automatically download the latest version (recommended)
   📁 2. Specify local file path manually

   - Please choose an option (1 or 2):

   ```

   ```

**Choose AppImage download option**

```

1

```

7. **When prompted for the icon filename**, type:

```

cursor-icon.png

```

Make sure the file exists in the `images` folder.

---

## ▶️ Launch Cursor

You can launch Cursor in one of the following ways:

- **From terminal:**

```bash
/opt/Cursor/AppRun
```

- **From applications menu:**
  - Press the Super (Windows) key
  - Search for “Cursor”
  - Click the icon to launch

---

## 🧹 Optional Cleanup

To delete the installer repo:

```bash
rm -rf Cursor-ubuntu
```

---

## 🔁 Uninstall Cursor

If you wish to remove Cursor:

```bash
./manage_cursor.sh uninstall
```

---

## 📁 Directory Structure

```
Cursor-ubuntu/
├── images/
│   └── cursor-icon.png
├── manage_cursor.sh
└── README.md
```

---

## 📢 Credits

- Cursor IDE: [https://www.cursor.sh](https://www.cursor.sh)
- Installer script by [@hieutt192](https://github.com/hieutt192)
