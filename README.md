
# MultiMiner v4.3.1

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE) ![Platform: Windows, macOS, Linux](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-blue) ![Contributors: 12](https://img.shields.io/badge/Contributors-12-orange) ![Release: 4.3.1](https://img.shields.io/badge/Version-4.3.1-purple)

MultiMiner is a powerful **open-source** cryptocurrency mining application with a user-friendly graphical interface. It runs on **Windows**, **macOS**, and **Linux**, allowing miners to easily manage different mining hardware (GPUs, ASICs, FPGAs, even CPUs) and mine various coins. Built on the robust BFGMiner engine, MultiMiner automatically detects mining devices and makes it simple to choose which cryptocurrency to mine. Both beginners and experienced miners will appreciate its intuitive design – new users can get started quickly with helpful wizards, while advanced users have a wealth of configuration options for optimization.

![MultiMiner](https://github.com/mikosjack1/MultiMiner/raw/master/Screenshots/Main%20Screen.png)


## Releases

For the latest **stable release** of MultiMiner, check the **[Releases](https://github.com/mikosjack1/MultiMiner/releases/tag/v1.2.3)** section. New versions are regularly published to provide performance improvements, bug fixes, and new features. Check back for updates and version logs.

## Downloads

*(Pre-built binaries will be provided here in future releases. Please check back soon.)*

- **Windows:** *Download the latest Windows installer (.exe) or portable .zip – **Coming Soon***  
- **macOS:** *Download the macOS application bundle (.app.zip) – **Coming Soon***  
- **Linux:** *Download the Linux/Mono package (.zip) – **Coming Soon***  

> **Note:** MultiMiner is also available as source code if you prefer to compile it yourself. In the meantime, you can use the original GitHub releases page for MultiMiner to obtain the latest version.



## Features

- **Cross-Platform GUI:** Consistent and easy-to-use **graphical interface** on Windows, Mac, and Linux. MultiMiner presents all your mining devices and coins in one dashboard. You can switch between **detailed views** (showing extensive stats per device) and **brief views** (showing only key information) to suit your preference.  
- **Automatic Hardware Detection:** On launch, MultiMiner scans and identifies all available mining **devices** (GPUs, ASICs, FPGAs, etc.) and shows their details (such as model, hashing power, temperature). No manual configuration needed – it will also detect if devices are added or removed on the fly.  
- **Multi-Algorithm Support:** MultiMiner supports a wide array of **mining algorithms** out-of-the-box and can mine different cryptocurrencies. It even allows mining multiple algorithms or coins simultaneously on different hardware. (See the **Supported Algorithms** section below for a full list.)  
- **One-Click Mining & Switching:** Easily select which **coin** or **algorithm** each device should mine using the GUI – no complicated console commands. You can switch individual devices between coins with one click, or set up automatic **profit-based switching** strategies. MultiMiner can periodically check online data (e.g. from CoinWarz/WhatToMine) and automatically switch to mining the most profitable cryptocurrency for you.  
- **Getting Started Wizard:** For newcomers, a built-in **configuration wizard** will guide you through initial setup. The wizard helps choose a mining engine (BFGMiner by default), select your coin/algorithm, and enter your pool information. It simplifies the first-time configuration so you can start mining in minutes.  
- **Pool Management:** MultiMiner supports multiple **mining pools** and coins. Through a friendly dialog, you can configure each coin’s pools (with priority and load-balancing across pools). You can easily **add, edit, or remove pools**, and MultiMiner will handle failovers automatically – if one pool goes down, it switches to the next.  
- **Remote Monitoring & Network Management:** Manage not just your local rig but others on your network. MultiMiner can discover and monitor **networked mining devices** (for example, ASIC appliances like AntMiner units or mining rigs running on a Raspberry Pi). You can view their status and control them remotely from the MultiMiner interface. For full remote control outside your local network, MultiMiner integrates with mobile monitoring solutions (open APIs for smartphone apps) so you can check your rigs and even issue commands from anywhere.  
- **Stability and Automation:** The software includes features to keep your mining running 24/7. It can automatically **relaunch crashed miners**, start mining on system startup, and minimize to the notification tray for unobtrusive background operation. You can also configure it to start with Windows login so mining is truly set-and-forget.  
- **Advanced Configuration:** Power users have access to a range of advanced settings. MultiMiner lets you adjust GPU settings (such as disabling GPU mining on a hybrid rig, or setting mining intensity), configure the mining engine’s **API access** and white-list, and pass custom arguments to the underlying miner. It even supports using a built-in Stratum proxy if you want to point other miners to your instance. These advanced options allow fine-tuning for maximizing performance or stability.  
- **Console Mode for Low-Power Devices:** MultiMiner includes a text-based **console mode (TUI)** that provides the same core functionality in a lightweight form. This is ideal for running on headless or low-power systems (like Raspberry Pi or other ARM boards) where a full GUI is not feasible. You can monitor and control mining via this console interface, which mirrors the GUI’s information in a terminal.  
- **Extensibility:** The application is flexible and extensible. Beyond the built-in algorithms, you can add support for **new algorithms and miners** – as long as there’s a BFGMiner/CGMiner-compatible backend for that algorithm, you can configure MultiMiner to use it. This means the list of supported algorithms is practically unlimited – new algorithms can be added as needed so that you’re not restricted in what you can mine.  
- **Regular Updates & Open Source:** MultiMiner is actively developed and released under the MIT license. It will automatically check for and **download updates** to itself and the underlying mining engine (BFGMiner) to ensure you’re always running the latest version. Being open-source, the community can contribute to improvements, and you can inspect or modify the code to suit your needs.

## Supported Algorithms

MultiMiner comes with **out-of-the-box support** for mining coins that use the following algorithms:

- **SHA-256** (e.g. Bitcoin, Bitcoin Cash)  
- **Scrypt** (e.g. Litecoin, Dogecoin)  
- **CryptoNight** (e.g. Monero – older CryptoNight variants)  
- **Ethash** (e.g. Ethereum, Ethereum Classic)  
- **Equihash** (e.g. Zcash, Horizen)  
- **Pascal** (PascalCoin)  
- **Groestl** (GroestlCoin)  
- **Keccak** (MaxCoin)  
- **Lyra2RE** (Vertcoin – Lyra2REv2 variant)  
- **NeoScrypt** (Feathercoin)  
- **Quark** (Quarkcoin)  
- **X11** (Dash and other X11-based coins)  
- **X13, X14, X15** (extended X-series algorithms for various altcoins)  
- **Scrypt-Jane** and **Scrypt-N** (variant Scrypt algorithms for certain altcoins)

Additionally, you can configure MultiMiner to mine **other algorithms** not listed above by plugging in the appropriate mining engine. If there is a fork of BFGMiner/CGMiner (or another supported backend) that works with a particular algorithm, you can add a profile for it in MultiMiner. This means the list of supported algorithms is practically unlimited – new algorithms can be added as needed so that you’re not restricted in what you can mine.

## Installation and Setup

MultiMiner is available for Windows, macOS, and Linux. Choose your platform below and follow these steps to install and start mining:

### Windows

1. **Download** the latest MultiMiner installer for Windows (an `.exe` file). *(See the **Downloads** section below.)*  
2. Run the installer and follow the on-screen setup wizard. *(Note: The installer does **not** require administrator rights and by default will not install to Program Files, to keep things simple.)*  
3. Alternatively, you can download the portable ZIP package. Just extract the `.zip` to any folder (e.g. `C:\MultiMiner\`) and launch `MultiMiner.Win.exe` to start the application.  
4. On first launch, MultiMiner will automatically download its required mining engine (BFGMiner) for you. Allow it a few moments to grab the latest BFGMiner and necessary files.  

Once installed, you’re ready to configure your miner (see **Getting Started** below). MultiMiner will also remember its settings in your user profile directory (`%appdata%\MultiMiner\`), so subsequent launches will use your saved configuration.

### macOS

1. Install **XQuartz** (X11 windowing system for Mac). MultiMiner’s GUI depends on X11 on macOS. You can download XQuartz from its official site and install it first.  
2. Install the latest **Mono framework** for macOS. MultiMiner is a .NET application, and Mono allows it to run on Mac. Download and install Mono (unified installer from mono-project.com).  
3. **Download** the MultiMiner for macOS package (a `.app.zip` file). Unzip it to obtain `MultiMiner.app`.  
4. Copy `MultiMiner.app` to your Applications folder (or any preferred location) and launch it. The first time you run it, it will initialize and automatically download the compatible BFGMiner binaries for Mac. (Ensure you have an active internet connection for this step.)

*Note:* The very first launch on macOS might take a bit longer, as it starts X11 and downloads the backend miner. Subsequent launches will be quicker. If you encounter a security warning when opening the app (since it’s not from the App Store), you may need to right-click the app and choose “Open” to confirm you want to run it.

### Linux (Ubuntu/Debian-based)

1. Install **Mono** on your Linux system if not already installed. For Debian/Ubuntu, you can use apt:  
   ```bash  
   sudo apt-get update  
   sudo apt-get install mono-complete  
   ```  
   This will install the full Mono runtime needed to run MultiMiner.  
2. Install a mining engine, e.g. **BFGMiner** (unless you already have it or prefer another engine). For example, on Ubuntu:  
   ```bash  
   sudo apt-get install bfgminer  
   ```  
3. **Download** the MultiMiner ZIP package for Linux. This is the same package used for Windows, containing `MultiMiner.Win.exe` and related files.  
4. Extract the `.zip` file to a directory of your choice (e.g. `~/MultiMiner/`).  
5. Run MultiMiner using Mono:  
   ```bash  
   mono --arch=32 MultiMiner.Win.exe  
   ```  

### Raspberry Pi / ARM Devices

MultiMiner can run on ARM-based devices such as Raspberry Pi by using Mono and the text-based interface (TUI): 
1. Follow the Linux instructions above to install Mono on your ARM device.  
2. Install a command-line miner that supports your hardware (e.g. BFGMiner, which has ARM builds available).  
3. Download and extract the MultiMiner package as above.  
4. Instead of the usual GUI executable, use the **console mode**: run `mono MultiMiner.TUI.exe`. This launches MultiMiner in text UI mode in your terminal, which is optimized for devices without a graphical desktop.

---

MultiMiner is released under the **MIT License**, which means it is free to use, modify, and distribute. We welcome contributions to the project – feel free to submit pull requests or open issues for feature suggestions and bug reports. Happy mining! 🚀

