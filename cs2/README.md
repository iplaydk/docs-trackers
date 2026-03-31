# Counter-Strike 2 (CS2) Tracker Setup Guide

## Table of Contents

1. [Overview](#overview)
2. [Prerequisites and Dependencies](#prerequisites-and-dependencies)
3. [Installation and Setup Instructions](#installation-and-setup-instructions)
   - [Step 1: Download and Install the CS2 Tracker](#step-1-download-and-install-the-cs2-tracker)
   - [Step 2: Configure CS2 and Game Settings](#step-2-configure-cs2-and-game-settings)
   - [Step 3: Using the Tracker During the Game](#step-3-using-the-tracker-during-the-game)
4. [Tracker Settings](#tracker-settings)
5. [Common Pitfalls and Best Practices](#common-pitfalls-and-best-practices)
6. [FAQ](#faq)

---

<a name="overview"></a>

## 1. Overview

The **CS2 Tracker** is a companion application used to track game and user data during specific events in **Counter-Strike 2**. It is designed to enhance the gaming experience by extracting real-time data and player statistics.

The primary use case for the Tracker is during gaming events and expos, such as Spillexpo, Dreamhack, and Gamebox Festival. This tracker integrates with the game and delivers accurate tracking data, allowing our partners to organize tournaments and challenges during an event.

This guide will walk you through the initial setup, usage, and best practices for integrating our Tracker with **CS2**. It covers everything from installation to troubleshooting, ensuring that new partners can get started quickly and experienced users can take full advantage of its features.

---

<a name="prerequisites-and-dependencies"></a>

## 2. Prerequisites and Dependencies

Before setting up the CS2 Tracker, ensure the following:

### Prerequisites:

- **Game**: Counter-Strike 2 installed and configured on your PC via Steam.
- **Operating System**: Windows 10 or higher (the tracker only supports Windows at this time).
- **Hardware**: Mobile phone with a QR code reader (e.g., the Camera app).

---

<a name="installation-and-setup-instructions"></a>

## 3. Installation and Setup Instructions

### <a name="step-1-download-and-install-the-cs2-tracker"></a> Step 1: Download and Install the CS2 Tracker

1. **Download the Tracker**:
   - Visit the provided link to download the CS2 Tracker.

2. **Installation Options**:

![run_anyway](https://github.com/user-attachments/assets/3da59261-236e-41e5-917d-bee8cc418914)

- When running the installer, Windows may display a security warning stating "Windows protected your PC" because the app doesn't have a verified publisher. Click on "More info" and then select "Run anyway" to proceed with the installation.
- During installation, select **"Anyone who uses this computer"** to make the tracker accessible for all user accounts.
- Choose a convenient installation location. This can be anywhere on your PC.

> **Note**: Do not open the tracker yet. Proceed to set up the game first.

3. **Taskbar Shortcut**:
   - Before launching the tracker, **pin it to the Windows Taskbar** for easy access. (optional)
   - The tracker will run in full-screen mode and cannot be closed from within the application. To close it, press the **Windows button** to open the taskbar, hover over the taskbar, and right-click the tracker to close.

---

### <a name="step-2-configure-cs2-and-game-settings"></a> Step 2: Configure CS2 and Game Settings

To ensure the tracker works correctly, you must configure **Counter-Strike 2** in a specific way. Follow the steps below:

1. **Set Steam Launch Options**:
   - Open **Steam** and navigate to your **Library**.
   - Right-click on **Counter-Strike 2** and select **Properties**.
   - In the **General** tab, find the **Launch Options** field.
   - Enter the following launch option:
     ```
     -condebug
     ```
   - Close the Properties window.

> **Important**: The `-condebug` launch option is essential. It enables console logging to a file, which is how the tracker reads game data. Without this option, the tracker will not be able to track any game data.

2. **Open the Game**:
   - Launch Counter-Strike 2 from Steam.

3. **Configure Display Settings**:
   - Go to **Settings** > **Video**.
   - Set **Display Mode** to **Fullscreen Windowed**.

> **Important**: The display mode **must** be set to **Fullscreen Windowed**. If the game is running in Exclusive Fullscreen, the tracker overlay will not appear on top of CS2, and the tracker will not function correctly.

4. **Configure Game Settings**:
   - Go to **Settings** > **Game**.
   - Set **Enable Developer Console (~)** to **Yes**.

5. **Subscribe to the Workshop Map**:
   - Open the Steam Workshop link provided by your iPlay contact.
   - Click **Subscribe** to add the map to your CS2 workshop collection.
   - The map will download automatically. You can verify it's installed by checking **Play** > **Workshop Maps** in CS2.

6. **Start the Workshop Map**:
   - In CS2, go to **Play** > **Practice** > **Workshop Maps**.
   - Select the subscribed workshop map from the list.
   - Press **Go** to start a local game on the map.

> **Important**: The tracker is designed to work with the specific workshop map provided for your event. Using a different map will result in the tracker not functioning correctly.

---

### <a name="step-3-using-the-tracker-during-the-game"></a> Step 3: Using the Tracker During the Game

1. **Open the Tracker**:
   - Once the workshop map has loaded, **Alt+Tab** to tab out of the game temporarily.

2. **Launch the CS2 Tracker**:
   - Open the tracker from the Windows Taskbar.
   - The tracker will display a **QR code**.
   - If the tracker appears to be running but the overlay is not showing, press **Ctrl + Shift + Alt + F** to force-reset the tracker.

> **Firewall Settings**: Windows might ask you to either allow or block the app through Windows Firewall. It is essential that you allow it through the Firewall as it connects to our online services. It's clear that there is a Firewall issue if the QR code isn't loading but it just keeps spinning.

3. **Configure the CS2 Tracker**
   - **Ctrl + Alt + O + P** allows you to configure the tracker.
   - The rest of the data is pre-configured on install for your event.
   - More information in step **4. Tracker Settings**

4. **Scan the QR Code**:
   - Use your mobile device to scan the code.

5. **Return to the Game**:
   - Press **Alt+Tab** to return to the game.

---

<a name="tracker-settings"></a>

## 4. Tracker Settings (pre-configured on install and optional)

The CS2 Tracker allows you to adjust specific tracking and reporting settings within the game. To access the settings, use the keyboard shortcut **Ctrl + Alt + O + P**. The following configurations are available:

1. **Data Settings**:
   - **Google Sheet Location** (optional): Select where the signup data should be stored for the challenge.
   - **Tracker store/location** (optional): Select what the current store / location is for the data to check with the challenge. E.g. Glostrup will then only send to the Glostrup leaderboard.

---

<a name="common-pitfalls-and-best-practices"></a>

## 5. Common Pitfalls and Best Practices

### Common Pitfalls:

- **Overlay Not Showing**: The tracker overlay only works if CS2 is running in **Fullscreen Windowed** mode. If you can't see the overlay, check your game's display settings and ensure it's not set to Exclusive Fullscreen.
- **Tracker Not Receiving Data**: If the tracker is not picking up any game data, verify that `-condebug` is set in the Steam launch options. Without this, the game does not write console output to a log file and the tracker has nothing to read.
- **Tracker Not Opening**: If the tracker does not open from the taskbar, ensure it was installed properly and try launching it again.
- **Full-Screen Tracker Locking You Out**: Since the tracker runs full-screen, it can lock you out of the desktop. To exit, use **Alt+Tab** or the **Windows button** to access the taskbar.
- **Overlay Not Disappearing After QR Scan**: If the QR code overlay doesn't disappear after scanning, you'll need to restart the tracker application. Don't worry about your settings - they will be remembered when you relaunch the app.

### Best Practices:

- **Taskbar Access**: Pin the tracker to the taskbar for easy access, especially during full-screen gaming sessions.
- **Pre-Game Setup**: Always configure your Steam launch options and game settings **before** opening the tracker.
- **Verify Launch Options**: Double-check that `-condebug` is present in the launch options every time you set up a new PC. It is the most common thing to forget.
- **Testing**: Run a few test rounds with staff or volunteers before starting official events to ensure the setup works seamlessly.

---

<a name="faq"></a>

## 6. FAQ

### Q1: What does `-condebug` do?

The `-condebug` Steam launch option tells CS2 to write all console output to a log file on disk. The tracker reads this log file to extract game data such as scores and match events. Without it, no data is captured.

### Q2: What should I do if the tracker locks my screen?

Since the tracker runs full-screen, use the **Alt+Tab** or **Windows button** to regain access to your desktop or taskbar. Worst case use **Alt+F4** if you know the tracker window is currently the active one.

### Q3: What do I do if the QR code doesn't scan?

Ensure that your QR scanner is working properly and that the tracker is running. The device must have a working internet connection (e.g., Wi-Fi or mobile data).

If the problem persists, try restarting the tracker or using another device to scan the code. In rare cases, older phones may fail to load the web app, preventing the QR overlay from registering the player.

### Q4: How can I test with many different users on my phone?

On iPhone and Safari, you can change to Private browsing before scanning the QR code. Then your phone will not remember your sign up.

---

This guide should give you everything you need to get the **CS2 Tracker** up and running with Counter-Strike 2. If you encounter issues that are not addressed here, consult the project's support team for further assistance.
