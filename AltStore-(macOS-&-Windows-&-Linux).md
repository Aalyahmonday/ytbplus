_The installation process is pretty straightforward. First, set up AltServer on your PC/Mac, use AltServer to install AltStore to your devices, then use AltStore to install uYouPlus. Your iDevice must be connected to your PC/mac during the whole process._

# Table of Content
* [Install AltStore](#install-altstore)
   * [ macOS](#-macos)
   * [⊞ Windows](#-windows)
   * [Linux](#-linux)
* [Installing uYouPlus](#installing-uyouplus)
* [Refresh uYouPlus](#refresh-uyouplus)
* [Troubleshooting](#troubleshooting)


# Install AltStore
##  macOS:
### 1. Requirements:
- macOS 10.14.4 and up.
- An iOS/iPadOS device running iOS 13 and later (because uYouPlus requires iOS/iPadOS 13+).
- An Apple account: you can use a spare account, but make sure that account was logged into a device before. Otherwise, you will get **_error_ _-22411_** (See https://github.com/rileytestut/AltStore/issues/175).

### 2. How to install AltStore (macOS):
- A very well-explained tutorial on how to install AltStore is available on the FAQ page of AltStore: [AltStore FAQ - macOS](https://faq.altstore.io/getting-started/how-to-install-altstore-macos)

### 3. After you successfully installed AltStore, head to [Installing uYouPlus!](#installing-uyouplus)

***
## ⊞ Windows:
### 1. Requirements:
- Windows 10 and up. (Windows 7 requires additional fix).
- iTunes and iCloud from Apple installed. **AltStore will not work with iTunes & iCloud from Microsoft Store**
  - iTunes: https://www.apple.com/itunes/download/win64
  - iCloud: https://updates.cdn-apple.com/2020/windows/001-39935-20200911-1A70AA56-F448-11EA-8CC0-99D41950005E/iCloudSetup.exe
- An iOS/iPadOS device running iOS 13 and later (because uYouPlus requires iOS/iPadOS 13+).
- An Apple account: you can use a spare account, but make sure that account was logged into a device before. Otherwise, you will get **_error_ _-22411_** (See https://github.com/rileytestut/AltStore/issues/175).

### 2. How to install AltStore (Windows):
- A very well-explained tutorial on how to install AltStore is available on the FAQ page of AltStore: [AltStore FAQ - Windows](https://faq.altstore.io/getting-started/how-to-install-altstore-windows)

### 3. After you successfully installed AltStore, head to [Installing uYouPlus!](#installing-uyouplus)
***

## 🐧 Linux
### AltServer-Linux
- AltServer doesn't support Linux by default. Thanks [@NyaMisty](https://twitter.com/MiscMisty) to port AltServer to Linux OS. AltServer-Linux is open source and you can see its source code here: https://github.com/NyaMisty/AltServer-Linux
- Since Linux is not my main OS, I'm afraid I can't help you much. However, if Linux is your main OS, I'm sure you know how to configure it properly.
- Note that you may need to compile from the source to build the latest version of AltServer-Linux.

### AltServer-LinuxGUI
- If you prefer GUI mode rather than CLI mode, [@powenn](https://twitter.com/powen00hsiao) made a GUI version of AltServer-Linux: https://github.com/powenn/AltServer-LinuxGUI

### ZSign
- ZSign is a cross platform signing tool that can run on macOS, Windows, and Linux. However, it’s not a user-friendly tool since it only has CLI mode. The instruction of ZSign is detailed here: https://github.com/zhlynn/zsign

***
# Installing uYouPlus
_✔︎ Now that you have AltStore installed on your iDevice, Let's start installing uYouPlus_
## 1. Configure AltStore:
- AltStore is installed on your phone, but you can't open it right now. To fix that, go to `Settings > General > Profile & Device Management`. There will be a profile with your account name in here. After you trust the profile, AltStore can be opened.
<p align="center" width="100%">
    <img width="50%" src="https://user-images.githubusercontent.com/52943116/157607556-fcf5e9d8-9187-4db9-a9da-3acd50f1ab9f.PNG">
</p>

- In AltStore, go to `Settings > Sign in with Apple ID`. Enter the Apple ID that was used to install AltStore. If AltStore says **“Could not find AltServer”**, then check if your phone is connected to Mac/PC.
<p align="center" width="100%">
    <img width="60%" src="https://user-images.githubusercontent.com/52943116/157608485-f72a2cc0-e42f-46bf-9c7b-c41ceeb5dd85.PNG">
</p>

- Congrats 🎉 You've just successfully configured AltStore.  

## 2. Install uYouPlus:
- Get the latest version of uYouPlus from the [Release page](https://github.com/qnblackcat/uYouPlus/releases/latest). I use Safari but you can use whatever you want to download the IPA. Select AltStore from the Share sheet. 
<p align="center" width="100%">
    <img width="70%" src="https://user-images.githubusercontent.com/52943116/157609122-17036f02-8122-4e74-bb14-ad03e186e090.PNG">
</p>

- **Remove App Extensions is not recommened** because it will remove the ability to use *Open in YouTube shortcut* & *Open in YouTube Extension* (https://github.com/CokePokes/YoutubeExtensions). uYouPlus will take 3 app IDs in total.  

<p align="center" width="100%">
    <img width="90%" src="https://user-images.githubusercontent.com/52943116/157610652-62f09dc6-18cd-4795-9895-1b1206cf5b7c.PNG">
</p>

- The process might take a few minutes. After that, you will uYouPlus on your Home Screen 🎉🎉🎉

### ☞ Other methods:

- Another method is use the [direct install link](https://github.com/qnblackcat/uYouPlus#download) on uYouPlus homepage. Simply open the link and let AltStore does its job. 
 
 - If you have access to AltStore beta, you can add my AltStore repo [here](https://qnblackcat.github.io/AltStore/).

# Refresh uYouPlus
- Unfortunately, apps that have been installed using non-developer Apple IDs are only valid for 7 days, and uYouPlus is not an exception. At which point it will no longer open (you'll see an error that says "**YouTube is no longer available**"). 
- To compensate for this, AltStore will periodically attempt to refresh uYouPlus in the background. In order for AltStore to do that, you must connect your phone with your Mac/PC via cable or Wi-fi. Then click **Refresh All** in **AltStore > My Apps**
- To enable Refresh Apps over Wi-fi. Make sure your phone and your mac/PC are on the same network.
  - **macOS:** Open Finder and enable “Show this iPhone when on WiFi” for your phone.
  - **Windows:** Open iTunes and enable iTunes Wi-Fi sync for your phone.

# Troubleshooting
- See https://altstore.io/faq/