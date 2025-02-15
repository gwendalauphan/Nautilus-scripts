# 📌 Nautilus Scripts Automation

## 📖 Description

**Enhance your Nautilus !!**
This repository provides scripts for Nautilus, accessible via **right-click**. The `setup.sh` script automates their installation by creating **symbolic links** to Nautilus.

---

## 🛠 How It Works

Nautilus executes scripts via **Right-click > Scripts** and provides environment variables:

- `$NAUTILUS_SCRIPT_SELECTED_FILE_PATHS` → Selected files
- `$NAUTILUS_SCRIPT_CURRENT_URI` → Current folder
- `$NAUTILUS_SCRIPT_SELECTED_URIS` → URIs of selected files

---

## 🔧 Installation

1️⃣ **Clone the repository**

```bash
git clone https://github.com/your-username/nautilus-scripts.git
cd nautilus-scripts
```

2️⃣ **Run the installation**

```bash
chmod +x setup.sh
./setup.sh
```

This script:
- Checks `scripts/`
- Creates `~/.local/share/nautilus/scripts` if necessary
- Adds symbolic links

3️⃣ **Usage**

- **Open Nautilus**
- **Right-click > Scripts > [Script Name]** 🚀

---

## 🗑 Uninstallation

```bash
rm ~/.local/share/nautilus/scripts/*
find ~/.local/share/nautilus/scripts/ -type l -delete
```

---

## 📌 Update

Add new scripts to `scripts/` and rerun:

```bash
./setup.sh
```

🚀 **Enjoy your Nautilus scripts!**


