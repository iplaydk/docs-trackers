# EA SPORTS™ F1® 24 Tracker Setup Guide

## Table of Contents

1. [Overview](#overview)
2. [Prerequisites and Dependencies](#prerequisites-and-dependencies)
3. [Installation and Setup Instructions](#installation-and-setup-instructions)
   - [Step 1: Download and Install the F1 24 Tracker](#step-1-download-and-install-the-f1-tracker)
   - [Step 2: Configure EA SPORTS™ F1® 24 and Game Settings](#step-2-configure-f1-and-game-settings)
   - [Step 3: Using the Tracker During the Game](#step-3-using-the-tracker-during-the-game)
4. [Tracker Settings](#tracker-settings)
5. [Common Pitfalls and Best Practices](#common-pitfalls-and-best-practices)
6. [FAQ](#faq)

---

<a name="overview"></a>

## 1. Overview

The **F1® 24 Tracker** is a companion application used to track race and telemetry data during specific events in **EA SPORTS™ F1® 24**. It is designed to enhance the competitive experience by extracting real-time data, lap times, and driver performances.

The primary use case for the Tracker is during gaming events/expos, such as Spillexpo, Dreamhack and Gamebox Festival. This tracker integrates with the game and delivers accurate tracking data, allowing our partners to organize tournaments and challenges during an event.

This guide will walk you through the initial setup, usage, and best practices for integrating our Tracker with **F1® 24**. It covers everything from installation to troubleshooting, ensuring that new partners can get started quickly and experienced users can take full advantage of its features.

---

<a name="prerequisites-and-dependencies"></a>

## 2. Prerequisites and Dependencies

Before setting up the F1® 24 Tracker, ensure the following:

### Prerequisites:

- **Game**: EA SPORTS™ F1® 24 installed and configured on your PC.
- **Operating System**: Windows 10 or higher (the tracker only supports Windows at this time).
- **Hardware**: Mobile Phone with QR code reader (f.e. Camera app).

---

<a name="installation-and-setup-instructions"></a>

## 3. Installation and Setup Instructions

### <a name="step-1-download-and-install-the-f1-tracker"></a> Step 1: Download and Install the F1 24 Tracker

1. **Download the Tracker**:

   - Visit the provided link to download the F1® 24 Tracker.

2. **Installation Options**:

   - When running the installer, Windows may display a security warning stating "Windows protected your PC" because the app doesn't have a verified publisher. Click on "More info" and then select "Run anyway" to proceed with the installation.
   - During installation, select **"Anyone who uses this computer"** to make the tracker accessible for all user accounts.
   - Choose a convenient installation location. This can be anywhere on your PC.

> **Note**: Do not open the tracker yet. Proceed to set up the game first.

3. **Taskbar Shortcut**:

   - Before launching the tracker, **pin it to the Windows Taskbar** for easy access. (optional)
   - The tracker will run in full-screen mode and cannot be closed from within the application. To close it, press the **Windows button** to open the taskbar, hover over the taskbar, and right-click the tracker to close.

---

### <a name="step-2-configure-f1-and-game-settings"></a> Step 2: Configure EA SPORTS™ F1® 24 and Game Settings

To ensure the tracker works correctly, you must configure **EA SPORTS™ F1® 24** in a specific way. Follow the steps below:

1. **Open the Game**:

   - Launch EA SPORTS™ F1® 24.

2. **Configure Display Settings**:

   - Go to **Settings** > **Graphics Settings**.
   - Go to **Video Mode**
   - Set the display mode to **Windowed (Fullscreen)** (very important for the tracker overlay to work).
   - Ensure the resolution matches your monitor's native resolution.

3. **Configure Telemetry Settings**:

![image (2)](https://github.com/user-attachments/assets/6f6bc029-2ed3-4561-8b23-5f694c6f934d)

   - Go to **Settings** > **Telemetry Settings**.
   - Set **UDP Telemetry** to **On**.
   - Set **UDP Broadcast Mode** to **Off**.
   - Set **UDP IP Address** to **127.0.0.1**.
   - Set **UDP Port** to **20777**.
   - Set **UDP Send Rate** to **20 Hz**.
   - Set **UDP Format** to **2024**.
   - Set **Your Telemetry** to **Public**.
   - Set **Show player names** to **Off**.

4. **Configure Racing Wheel** (for Logitech G29/G920/other wheels):

   - Go to **Settings** > **Controls, Vibration & Force Feedback**.
   - Select your Racing wheel from the device list, press **Enter** then **Edit**.
   - Find the button currently assigned to **Pause**.
   - Select this button and change its assignment to **ESC** on your keyboard (not racing wheel).
   - This ensures participants can only exit the game using the keyboard ESC key, preventing accidental exits during races.
   - Apply and save these settings.

5. **Set Up Time Trial Parameters**:

   - In the main menu select **F1 World** and press **Play**.
   - Select **Time Trial** from the list and then **F1 2024** from the next screen.
   - Select the team (**McLaren** or as specified for your event).
   - Choose a track (**Monza** or as specified for your event).
   - Time Trial mode allows unlimited laps and never ends until the player exits.
   - Once the loading is done press **Go to track** and then **Flying lap**.

---

### <a name="step-3-using-the-tracker-during-the-game"></a> Step 3: Using the Tracker During the Game

1. **Open the Tracker**:

   - Once the race begins, **press `Esc`** to pause the game.
   - **Alt+Tab** to tab out of the game temporarily.

2. **Launch the F1® 24 Tracker**:

   - Open the tracker from the Windows Taskbar.
   - The tracker will display a **QR code**.

> **Firewall Settings**: Windows might ask you to either allow or block the app through Windows Firewall. It is essential that you allow it through the Firewall as it connects to our online services.

3. **Configure the F1® 24 Tracker**

   - **Ctrl + Alt + O + P** allows you to configure the tracker.
   - First time, set the Google Sheet Tab to the wrong Sheet. Press **Save** and then re-save with the right one. This is to ensure that the data is sending correctly.
   - The rest of the data is pre-configured on install for your event.
   - More information in step **4. Tracker Settings**

4. **Scan the QR Code**:

   - Use your mobile device to scan the code.

5. **Return to the Game**:

   - Press **Alt+Tab** to return to the Forza game.

> **Important**: The first round should be played by a staff member as the initial round will have incorrect timing. After the first round, tracking will operate accurately for all future races.

---

<a name="tracker-settings"></a>

## 4. Tracker Settings (pre-configured on install and optional)

![f1-tracker-settings](https://github.com/user-attachments/assets/87485793-198c-4537-b6dd-4a294b1ddffa)

The F1® 24 Tracker allows you to adjust specific tracking and reporting settings within the game. To access the settings, use the keyboard shortcut **Ctrl + Alt + O + P**. The following configurations are available:

1. **Race Parameters**:

   - **Total Laps**: Set the maximum number of laps each user can complete in a session before the QR code reappears.
   - **Maximum Time (Minutes)**: Define the maximum time limit for each race session before the QR code reappears.

---

<a name="common-pitfalls-and-best-practices"></a>

## 5. Common Pitfalls and Best Practices

### Common Pitfalls:

- **Overlay Not Working**: The tracker overlay only works if F1® 24 is running in **Fullscreen Windowed** mode. If you can't see the overlay, check your game's display settings and ensure it's not set to Exclusive Fullscreen.
- **Tracker Not Opening**: If the tracker does not open from the taskbar, ensure it was installed properly and try launching it again.
- **Incorrect Timing in First Race**: Always remember that the first race will not be timed correctly. After the initial round, the system will function as expected.
- **Full-Screen Tracker Locking You Out**: Since the tracker runs full-screen, it can lock you out of the desktop. To exit, use **Alt+Tab** or the **Windows button** to access the taskbar.
- **Overlay Not Disappearing After QR Scan**: If the QR code overlay doesn't disappear after scanning, you'll need to restart the tracker application. Don't worry about your settings - they will be remembered when you relaunch the app.

### Best Practices:

- **Taskbar Access**: Pin the tracker to the taskbar for easy access, especially during full-screen gaming sessions.
- **Pre-Game Setup**: Always configure your race and car settings **before** opening the tracker.
- **Testing**: Run a few test races with staff or volunteers before starting official events to ensure the setup works seamlessly.

---

<a name="faq"></a>

## 6. FAQ

### Q1: Why is my first race time incorrect?

The first race is used to calibrate the tracker. Times for the first round are inaccurate, but all subsequent races will be tracked correctly.

### Q2: Can I use the tracker with any car?

Technically, yes. But remember to adjust it according to your race settings. **McLaren 1976 #11 M23**.

### Q3: What should I do if the tracker locks my screen?

Since the tracker runs full-screen, use the **Alt+Tab** or **Windows button** to regain access to your desktop or taskbar.

### Q4: Can I configure my own race settings?

While it's possible to adjust settings in Forza, the tracker is optimized for the configurations provided in this guide. Deviating from the recommended setup may result in inaccurate tracking data.

### Q5: What do I do if the QR code doesn’t scan?

Ensure that your QR scanner is working properly and that the tracker is running. It is important that the device has a working internet connection (F.e. WiFi or 3G/4G/5G).

If the problem persists, try restarting the tracker or using another device to scan the code.

### Q6: How can I test with many different users on my phone?

On iPhone and Safari, you can change to Private browsing before scanning the QR code. Then your phone will not remember your sign up.

---

This guide should give you everything you need to get the **F1® 24 Tracker** up and running with EA SPORTS™ F1® 24. If you encounter issues that are not addressed here, consult the project’s support team for further assistance.
