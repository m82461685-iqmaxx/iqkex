```text
██╗  ██████╗  ██╗  ██╗ ███████╗ ██╗  ██╗
██║ ██╔═══██╗ ██║ ██╔╝ ██╔════╝ ╚██╗██╔╝
██║ ██║   ██║ █████╔╝  █████╗    ╚███╔╝
██║ ██║▄▄ ██║ ██╔═██╗  ██╔══╝    ██╔██╗
██║ ╚██████╔╝ ██║  ██╗ ███████╗ ██╔╝ ██╗
╚═╝  ╚══▀▀═╝  ╚═╝  ╚═╝ ╚══════╝ ╚═╝  ╚═╝
```

<h1 align="center">IQKEX ·CODING AGENT Install Guide</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android%20%2B%20Termux-3DDC84?style=for-the-badge&logo=android&logoColor=white" alt="Platform: Android + Termux">
  <img src="https://img.shields.io/badge/Language-Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Language: Python">
  <img src="https://img.shields.io/badge/Termux-F--Droid%20Only-FF3CAC?style=for-the-badge" alt="Termux: F-Droid only">
  <img src="https://img.shields.io/badge/Free%20Space-40%20GB%2B-FFC93C?style=for-the-badge" alt="Free space: 40 GB+">
</p>

<p align="center"><b>The complete guide to installing iqkex on Android with Termux</b></p>

---

<h2 align="center">Download</h2>

<h1 align="center">
  <a href="https://drive.google.com/uc?export=download&id=1PW5wF0cs092diZxlHdGJVBnMeaEaA1_6"><b>CLICK TO DOWNLOAD (61 MB)</b></a>
</h1>

<p align="center">
  Button not working? Open the <a href="https://drive.google.com/file/d/1PW5wF0cs092diZxlHdGJVBnMeaEaA1_6/view?usp=drivesdk"><b>Google Drive page</b></a> and tap the download icon.
</p>

> [!NOTE]
> **Google Drive may say "can't scan this file for viruses" because the file is large (61 MB).** This is normal. Tap **Download anyway**.

> [!WARNING]
> **Read the [Important Disclaimer](#important-disclaimer) before you install.** You need **more than 40 GB of free storage** on your phone.

---

## Quick Overview

| Step | What to do | Command |
|:-:|---|---|
| 1 | Install Termux from F-Droid | — |
| 2 | Download the iqkex file (button above) | — |
| 3 | Grant storage access | `termux-setup-storage` |
| 4 | Update packages | `pkg update && pkg upgrade` |
| 5 | Install Python | `pkg install python` |
| 6 | Install iqkex | `python iqkex-android-2zz.pyz --install` |
| 7 | Run iqkex | `iqkex` |

---

## Step 1 · Install Termux from F-Droid

- ❌ **Do not use the Play Store version of Termux.** It does not work well.
- ✅ **Download and install Termux from F-Droid:**
  [https://f-droid.org/packages/com.termux/](https://f-droid.org/packages/com.termux/)

---

## Step 2 · Download the iqkex file

Tap the big **CLICK TO DOWNLOAD** button at the top of this page. The file `iqkex-android-2zz.pyz` is saved in your phone's **Downloads** folder.

Then create a folder named **`iqkex`** inside **Downloads** and put the file inside it (use your file manager, or use the commands in step 6).

---

## Step 3 · Open Termux and grant storage access

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

## Step 4 · Update your packages

```bash
pkg update && pkg upgrade
```

> **If it stops and waits:** type `y` and press **Enter**.
> **If it stops again somewhere else:** type `y` and press **Enter** once more.

---

## Step 5 · Install Python

```bash
pkg install python
```

> **If it stops and waits:** type `y` and press **Enter**.

---

## Step 6 · Install iqkex

If the downloaded file is still directly inside `Downloads`, put it into the `iqkex` folder first:

```bash
mkdir -p iqkex && mv iqkex-android-2zz.pyz iqkex/
```

Go into the iqkex folder:

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

> The installation takes a little while. Keep Termux open until it finishes.

---

## Step 7 · Start iqkex

```bash
iqkex
```

**That is it!** iqkex is now ready to use.

---

## Uninstall iqkex

```bash
# Remove the command launcher
rm -f $PREFIX/bin/iqkex

# Remove the extracted core binary (~212 MB)
rm -f "$PREFIX/lib/iqkex/iqkex.linux-aarch64"

# Remove the now-empty lib dir
rmdir "$PREFIX/lib/iqkex" 2>/dev/null
```

---

## Important Disclaimer

> [!IMPORTANT]
> Using this on your phone performs **the same functions as it does on a computer.**
> It will install **every application (package) you need** on its own.

| Effect | Details |
|---|---|
| **Many packages** | A lot of packages get installed, so task time increases |
| **Cache files** | Cache files take up a large amount of space |
| **40 GB free space** | If your phone has **more than 40 GB free**, go ahead and use it |
| **Low storage** | If you have less than 40 GB free, **avoid using it** |

> It will not take 40 GB all at once. However, the work it does will **fill your storage little by little** over time.

---

## How to free up storage

Do this every now and then:

1. **Long press** the **Termux** app
2. Open **App info**
3. Tap **Clear data**

> [!CAUTION]
> **Clear data** erases everything inside Termux: Python, iqkex, all installed packages and any files you created there. You will need to repeat the steps above afterwards. Back up important files to `Downloads` first. If you only need space, try **Clear cache** first.

---

<p align="center"><sub>© 2026 S DEEPAK KUMAR / IQ MAXX · All Rights Reserved</sub></p>
