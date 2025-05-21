# Forza Motorsport (Forza) Tracker Setup Guide

## Table of Contents

1. [Overview](#overview)
2. [Prerequisites and Dependencies](#prerequisites-and-dependencies)
3. [Installation and Setup Instructions](#installation-and-setup-instructions)
   - [Step 1: Download and Install the Forza Tracker](#step-1-download-and-install-the-forza-tracker)
   - [Step 2: Configure Forza and Game Settings](#step-2-configure-forza-and-game-settings)
   - [Step 3: Using the Tracker During the Game](#step-3-using-the-tracker-during-the-game)
4. [Tracker Settings](#tracker-settings)
5. [Common Pitfalls and Best Practices](#common-pitfalls-and-best-practices)
6. [FAQ](#faq)

---

<a name="overview"></a>

## 1. Overview

The **Forza Tracker** is a companion application used to track race and telemetry data during specific events in **Forza Motorsport**. It is designed to enhance the competitive experience by extracting real-time data, lap times, and driver performances.

The primary use case for the Tracker is during gaming events/expos, such as Spillexpo, Dreamhack and Gamebox Festival. This tracker integrates with the game and delivers accurate tracking data, allowing our partners to organize tournaments and challenges during an event.

This guide will walk you through the initial setup, usage, and best practices for integrating our Tracker with **Forza**. It covers everything from installation to troubleshooting, ensuring that new partners can get started quickly and experienced users can take full advantage of its features.

---

<a name="prerequisites-and-dependencies"></a>

## 2. Prerequisites and Dependencies

Before setting up the Forza Tracker, ensure the following:

### Prerequisites:

- **Game**: Forza Motorsport installed and configured on your PC.
- **Operating System**: Windows 10 or higher (the tracker only supports Windows at this time).
- **Hardware**: Mobile Phone with QR code reader (f.e. Camera app).

---

<a name="installation-and-setup-instructions"></a>

## 3. Installation and Setup Instructions

### <a name="step-1-download-and-install-the-forza-tracker"></a> Step 1: Download and Install the Forza Tracker

1. **Download the Tracker**:

   - Visit the provided link to download the Forza Tracker.

2. **Installation Options**:

   - When running the installer, Windows may display a security warning stating "Windows protected your PC" because the app doesn't have a verified publisher. Click on "More info" and then select "Run anyway" to proceed with the installation.
   - During installation, select **"Anyone who uses this computer"** to make the tracker accessible for all user accounts.
   - Choose a convenient installation location. This can be anywhere on your PC.

> **Note**: Do not open the tracker yet. Proceed to set up the game first.

3. **Taskbar Shortcut**:

   - Before launching the tracker, **pin it to the Windows Taskbar** for easy access. (optional)
   - The tracker will run in full-screen mode and cannot be closed from within the application. To close it, press the **Windows button** to open the taskbar, hover over the taskbar, and right-click the tracker to close.

---

### <a name="step-2-configure-forza-and-game-settings"></a> Step 2: Configure Forza and Game Settings

To ensure the tracker works correctly, you must configure **Forza Motorsport** in a specific way. Follow the steps below:

1. **Open the Game**:

   - Launch Forza Motorsport and navigate to **Play** > **Main Menu** > **Race** > **Free Play** > **Advanced Event Setup**.

2. **Data Out Settings**:
   ![dataOut](https://github.com/user-attachments/assets/34a7afdf-a689-43e9-81f4-edad603fef13)

   - Go to **Settings** > **Gameplay & HUD** and scroll to the bottom.
   - Set **Data Out** to **On**.
   - **Data Out IP Address** should be set to **127.0.0.1**.
   - **Data Out Port** should be set to **9966**.
   - **Car Out Packet Format** should be set to **Car Dash**.

3. **Choose a Car**:

   - In the car selection menu, select **Buy or Rent Cars**.
   - Choose the **McLaren 1976 #11 M23** and select **Rent**.

4. **Set Up Race Parameters**:

   - Race Type: **Circuit Race**
   - Track: **Custom** > **Grand Oak Raceway, Club Circuit**
   - Laps: **999**
   - Time: **Noon**
   - Start: **Rolling**
   - Track Rubber: **Off**
   - Weather: **Clear**
   - Drivatars: **0**

5. **Rules Settings**:

   - Rules Preset: **Custom**
   - Damage: **Cosmetic Only**
   - Penalty: **Moderate**
   - Rewind: **Off**
   - Race Start: **Rolling**

6. **Additional Configurations**:

   - Fuel & Tire: **Fuel 100%**
   - Driving Assists: **Moderate**

7. **Start the Race**:
   - Accept all settings and begin the race.
   - Wait for the countdown to end and the race to start.

---

### <a name="step-3-using-the-tracker-during-the-game"></a> Step 3: Using the Tracker During the Game

1. **Open the Tracker**:

   - Once the race begins, **press `Esc`** to pause the game.
   - **Alt+Tab** to tab out of the game temporarily.

2. **Launch the Forza Tracker**:

   - Open the tracker from the Windows Taskbar.
   - The tracker will display a **QR code**.

> **Firewall Settings**: Windows might ask you to either allow or block the app through Windows Firewall. It is essential that you allow it through the Firewall as it connects to our online services.

3. **Configure the Forza Tracker**

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

![forza-tracker-settings](https://github.com/user-attachments/assets/87485793-198c-4537-b6dd-4a294b1ddffa)

The Forza Tracker allows you to adjust specific tracking and reporting settings within the game. To access the settings, use the keyboard shortcut **Ctrl + Alt + O + P**. The following configurations are available:

1. **Google Sheet Tab**: Specify the Google Sheet tab where user information should be sent. The Google Sheet document is pre-defined.

2. **Race Parameters**:

   - **Total Laps**: Set the maximum number of laps each user can complete in a session before the QR code reappears.
   - **Maximum Time (Minutes)**: Define the maximum time limit for each race session before the QR code reappears.

3. **Conditional Data Submission**:
   - **Track Name**: Specify the track name required for data submission.
   - **Car Name**: Define the car name that must be used to validate data submission.
   - **Fuel Level**: Set the minimum required fuel level for a lap to be recorded.
   - **Invalid Laps**: Toggle whether or not laps marked as invalid (e.g., for track cutting) should be included in the submission.
   - **Lap Time Filter**: Set a lap time threshold to exclude laps that are above or below a specified number of seconds.

---

<a name="common-pitfalls-and-best-practices"></a>

## 5. Common Pitfalls and Best Practices

### Common Pitfalls:

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

This guide should give you everything you need to get the **Forza Tracker** up and running with Forza Motorsport. If you encounter issues that are not addressed here, consult the project’s support team for further assistance.
