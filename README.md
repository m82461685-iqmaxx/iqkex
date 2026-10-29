<img src="assets/developer.svg" align="right" width="250" alt="Developer coding at a desktop">

<p align="center">
  <img src="assets/banner.svg" width="640" alt="IQKEX Termux Install Guide">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android%20%2B%20Termux-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Android">
  <img src="https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Termux-F--Droid%20Only-FF3CAC?style=for-the-badge" alt="F-Droid">
  <img src="https://img.shields.io/badge/Free%20Space-40%20GB%2B-FFC93C?style=for-the-badge" alt="40 GB">
</p>

<h3 align="center">🐍 The complete guide to installing iqkex on Android with Termux 🦅</h3>

<br clear="right">

> [!WARNING]
> **Read the [Important Disclaimer](#-important-disclaimer) before you install.** You need **more than 40 GB of free storage** on your phone.

---

## 📋 Quick Overview

| Step | What to do | Command |
|:-:|---|---|
| 1️⃣ | Install Termux from F-Droid | — |
| 2️⃣ | Grant storage access | `termux-setup-storage` |
| 3️⃣ | Update packages | `pkg update && pkg upgrade` |
| 4️⃣ | Install Python | `pkg install python` |
| 5️⃣ | Install iqkex | `python iqkex-android-2zz.pyz --install` |
| 6️⃣ | Run iqkex | `iqkex` |

---

<img src="assets/h-install.svg" width="820" alt="Step 1 Install Termux">

### 1️⃣ Install Termux from F-Droid

- ❌ **Do not use the Play Store version of Termux.** It does not work well.
- ✅ **Download and install Termux from F-Droid:**
  👉 [https://f-droid.org/packages/com.termux/](https://f-droid.org/packages/com.termux/)

---

<img src="assets/h-storage.svg" width="820" alt="Step 2 Storage Access">

### 2️⃣ Open Termux and grant storage access

Open Termux and run this command. When the permission prompt appears, tap **Allow**:

```bash
termux-setup-storage
```

Next, move into your Downloads folder. Press **Enter** after each line:

```bash
cd storage
```

```bash
cd Downloads
```

---

<img src="assets/h-update.svg" width="820" alt="Step 3 Update Packages">

### 3️⃣ Update your packages

```bash
pkg update && pkg upgrade
```

> 💡 **If it stops and waits:** type `y` and press **Enter**.
> 🔁 **If it stops again somewhere else:** type `y` and press **Enter** once more.

---

<img src="assets/h-python.svg" width="820" alt="Step 4 Install Python">

### 4️⃣ Install Python

```bash
pkg install python
```

> 💡 **If it stops and waits:** type `y` and press **Enter**.

---

<img src="assets/h-iqkex.svg" width="820" alt="Step 5 Install iqkex">

### 5️⃣ Install iqkex

First, go into the iqkex folder:

```bash
cd iqkex
```

Then run the install command:

```bash
python iqkex-android-2zz.pyz --install
```

You will see a message like this:

```text
[ iqkex ]  unpacking core..
```

> ⏳ The installation takes a little while. Keep Termux open until it finishes.

---

<img src="assets/h-run.svg" width="820" alt="Step 6 Run iqkex">

### 6️⃣ Start iqkex

```bash
iqkex
```

🎉 **That is it!** iqkex is now ready to use.

---

<img src="assets/h-demo.svg" width="820" alt="Live Terminal Demo">

<p align="center">
  <img src="assets/terminal.svg" width="820" alt="Animated terminal demo">
</p>

---

<img src="assets/h-uninstall.svg" width="820" alt="Uninstall">

### 🗑️ Uninstall iqkex

To remove iqkex, use the commands below:

```bash
# Remove the command launcher
rm -f $PREFIX/bin/iqkex

# Remove the extracted core binary (~212 MB)
rm -f "$PREFIX/lib/iqkex/iqkex.linux-aarch64"

# Remove the now-empty lib dir
rmdir "$PREFIX/lib/iqkex" 2>/dev/null
```

---

<a id="-important-disclaimer"></a>
<img src="assets/h-warning.svg" width="820" alt="Important Disclaimer">

### ⚠️ Important Disclaimer

> [!IMPORTANT]
> Using this on your phone performs **the same functions as it does on a computer.**
> It will install **every application (package) you need** on its own.

| ⚡ Effect | 📝 Details |
|---|---|
| 📦 **Many packages** | A lot of packages get installed, so task time increases |
| 🗂️ **Cache files** | Cache files take up a large amount of space |
| 💾 **40 GB free space** | If your phone has **more than 40 GB free**, go ahead and use it |
| 🚫 **Low storage** | If you have less than 40 GB free, **avoid using it** |

> 📌 It will not take 40 GB all at once. However, the work it does will **fill your storage little by little** over time.

---

<img src="assets/h-clean.svg" width="820" alt="Free up storage">

### 🧹 How to free up storage

Do this every now and then:

1. 📱 **Long press** the **Termux** app
2. ℹ️ Open **App info**
3. 🗑️ Tap **Clear data**

> [!CAUTION]
> **Clear data** erases everything inside Termux: Python, iqkex, all installed packages and any files you created there. You will need to repeat the steps above afterwards. Back up important files to `Downloads` first. If you only need space, try **Clear cache** first.

---

<p align="center">
  <b>🦅 Fly high &nbsp;·&nbsp; 🐍 Code smart &nbsp;·&nbsp; 💻 Build more</b><br>
  <sub>© 2026 S DEEPAK KUMAR / IQ MAXX · All Rights Reserved</sub>
</p>
