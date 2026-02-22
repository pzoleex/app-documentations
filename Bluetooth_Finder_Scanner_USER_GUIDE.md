# Bluetooth Scanner - User Guide

Welcome to Bluetooth Scanner! This app lets you discover, identify, and manage all Bluetooth devices around you. Whether you want to find a lost earbud, check your headphone's audio codec, or see what Bluetooth devices are nearby, this guide will walk you through every feature.

---

## Table of Contents

1. [Introduction](#1-introduction)
2. [Getting Started](#2-getting-started)
3. [Scanning for Devices](#3-scanning-for-devices)
4. [Device Actions](#4-device-actions)
5. [Paired Devices Tab](#5-paired-devices-tab)
6. [Filters Tab](#6-filters-tab)
7. [Device Finder](#7-device-finder)
8. [GPS Location Tracking (Android 13+)](#8-gps-location-tracking-android-13)
9. [History Tab](#9-history-tab)
10. [Charts Tab](#10-charts-tab)
11. [User-Defined Device Types](#11-user-defined-device-types)
12. [Settings](#12-settings)
13. [Navigation Drawer](#13-navigation-drawer)
14. [Free vs Extreme Edition](#14-free-vs-extreme-edition)
15. [Tips and Notes](#15-tips-and-notes)

---

## 1. Introduction

Bluetooth Scanner is a powerful Android app that scans for nearby Bluetooth devices and displays detailed information about each one — including the device name, type, manufacturer, signal strength, supported services, audio codecs, battery level, and more.

**Key capabilities:**

- Discover all Bluetooth devices in your surroundings (Classic and BLE)
- Identify device types automatically (headphones, phones, laptops, smartwatches, and 40+ other categories)
- Locate a lost Bluetooth device using the signal strength finder
- Track the last known GPS location of your Bluetooth devices (Android 13+)
- View audio codec details and control connected audio devices
- Keep a history of past scans with charts and statistics
- Filter and sort discovered devices in many different ways

The app is available in two editions:

- **Free Edition** — Full scanning and basic features with ads
- **Extreme Edition** — Unlocks advanced filters, export, unlimited customization, protocol selection, and removes ads

---

## 2. Getting Started

### First Launch

When you open the app for the first time, you will be asked to grant a few permissions:

1. **Nearby Devices permission** — Required so the app can scan for Bluetooth devices. Tap **"Grant permission"** to allow it.
2. **Location permission** — On some Android versions, Bluetooth scanning requires location access. Tap **"Grant permission"** to enable full functionality. You can also choose **"Continue without it"**, but some features may not work.
3. **Data collection opt-in** — You will be asked if you want to help improve the app by sending basic crash and usage data to the developer. This is optional — tap **"Accept"** or **"Decline"**.

> **Tip:** If Bluetooth is turned off on your device, the app will ask you to enable it.

### Main Screen Overview

The main screen has several areas:

- **Toolbar** (top) — Contains the Bluetooth adapter toggle and the overflow menu (three dots) with access to Settings and Purchase.
- **Navigation drawer** (swipe from the left edge) — Quick access to Settings, Theme, Purchase, Subscriptions, EULA, and Privacy Policy.
- **Tab bar** — Six tabs for navigating different sections:
  - **Devices** — Scanned device list (main view)
  - **Paired** — Your paired/bonded devices
  - **Filters** — Filter and sort the device list
  - **History** — Past scan sessions
  - **Charts** — Visual statistics
  - **About** — App info and developer links
- **Bottom button bar** — Three buttons: **Adapter info**, **Start/Stop**, and **Clear**.

---

## 3. Scanning for Devices

### Starting a Scan

1. Make sure Bluetooth is enabled on your device.
2. Tap the **Start** button at the bottom of the screen.
3. The app will begin scanning and devices will appear in the list as they are discovered.
4. Tap **Stop** to end the scan.
5. Tap **Clear** to remove all discovered devices from the list.

> **Tip:** Start the scan multiple times to detect all nearby devices. Some devices may not respond to the first scan.

### What Each Device Card Shows

Each discovered device displays:

- **Device name** — The Bluetooth name (or "Unknown" if not available)
- **Device type icon** — Automatically detected category (headphone, phone, laptop, etc.)
- **Bluetooth address** — The unique MAC address of the device
- **Connection status** — Shows "(Connected)" or "(Paired)" if applicable
- **RSSI signal strength** — The signal power in dBm, with a quality label:
  - **Amazing** (very strong), **Good**, **OK**, **Weak**, or **Bad**
- **Vendor/Manufacturer** — Identified from the Bluetooth registry (e.g., "Apple, Inc.", "Samsung Electronics")
- **Services** — What the device supports (Audio, Telephony, Networking, etc.)
- **Protocol** — Classic (BR/EDR), BLE only, or Dual mode
- **Battery level** — If the device reports it
- **Audio codec info** — For connected audio devices: codec name, sample rate, bit depth, and max bit rate
- **"It seems to be original (not fake)"** — Shown for Apple devices when the app's originality check passes
- **First seen / Last seen** — Timestamps of when the device was first and last detected

### Compact View

You can switch to a more condensed device list in **Settings > Enable compact view**. This shows less detail per device but lets you see more devices at once. You can also set the number of columns (1–3) for portrait and landscape modes.

---

## 4. Device Actions

Tap on any device in the list to expand its detail panel. The following action buttons are available:

### Customize

Change how the device appears in your list:

- **Rename** — Set a custom display name
- **Change device type** — Pick from 40+ built-in types or your own custom types
- **Play beep when found** — The app will play a sound whenever this device is detected during a scan
- **Pin to top** — Keep this device at the top of the list
- **Hide from future search** — Remove the device from future scan results (can be undone in Settings)
- Tap **Save** to apply changes, or **Reset** to revert

> In the Free edition, you can customize up to 2 devices. The Extreme edition allows unlimited customization.

### Details

View in-depth technical information:

- Device class codes and group classification
- Connection encryption status
- Noise reduction and voice recognition support (for headsets)
- Current audio codec configuration (codec name, sample rate, bit depth, bit rate)
- List of codecs supported by the phone and the headphone
- Device UUIDs (service identifiers)
- BLE GATT characteristics (serial number, firmware version, model, manufacturer, etc.)

### Pair / Unpair

- **Pair** — Initiate Bluetooth pairing with the device
- **Forget** — Remove the pairing (only works for devices paired through this app)

### Find

Opens the **Device Finder** dialog — see [Section 7](#7-device-finder) for full details.

### Audio Control

Available for connected audio (A2DP) devices. Opens a control panel with:

- **Connect / Disconnect** — Manage the audio connection (this does not unpair the device)
- **Set as active** — Choose this device as the active audio output (useful when multiple audio devices are connected)
- **Volume slider** — Adjust the device volume
- **Media controls** — Play/Pause, Previous track, Next track
- **Change codec** — Switch between supported audio codecs (SBC, AAC, aptX, aptX HD, LDAC) with options for sample rate and bit depth

> Audio Control is a beta/experimental feature. Most headphones support SBC; some also support aptX or AAC.

### Codec Compare

Shows a horizontal bar chart comparing the maximum bit rates of common Bluetooth audio codecs (SBC, AAC, aptX, aptX HD, LDAC, SSC). Your current codec is highlighted. Only visible for connected audio devices.

### Copy / Share

Copies the device's information to your clipboard or shares it via any app (email, messaging, etc.). Includes: name, type, MAC address, audio info, services, codecs, RSSI, protocol, vendor, battery, and first seen date.

> The Free edition shares a limited summary. The Extreme edition shares full details.

---

## 5. Paired Devices Tab

The **Paired** tab shows all Bluetooth devices currently paired (bonded) with your phone. This list comes directly from your Android Bluetooth settings.

- Tap a device to see its details and available actions
- Use the **Refresh** button to update the list
- Use the **Open Bluetooth Settings** button to go to your phone's Bluetooth settings page

---

## 6. Filters Tab

The Filters tab lets you narrow down the scanned device list. Multiple filters can be combined — a device must match **all** active filters to appear.

### Device Type Group Filters

Toggle switches to show or hide entire device categories:

- **Computer** — Laptops, MacBooks, smart boxes, GPS devices
- **Phone** — Phones, tablets, iPhones
- **Health** — Blood pressure monitors, glucose meters, weighing scales, pulse oximeters
- **Wearable** — Smartwatches, smart bands, smart glasses
- **Audio-Video** — Headphones, headsets, speakers, earbuds, cameras, smart TVs
- **Peripheral** — Keyboards, mice, printers, scanners, selfie sticks
- **Unknown** — Unclassified devices

### Show Only New Devices

When enabled, only devices seen for the first time in the current scan session are shown.

### Date Range Filter

Filter devices by when they were first detected:

- **Any** (default) — Show all
- **Last 24 hours**
- **Last 7 days**
- **Last 30 days**

### Sort / Order Options

Sort the device list by:

- No ordering (discovery order)
- **RSSI** (signal strength)
- **Bluetooth address**
- **Name** (alphabetical)
- **Vendor** (alphabetical)
- **First seen time** (chronological)
- **Connected first** (paired devices at top)

Use the **Reverse order** toggle to flip the sort direction (e.g., A–Z becomes Z–A).

### Exclude Unknown Name / Vendor

- **Exclude unknown name** — Hide devices that don't broadcast a name
- **Exclude unknown vendor** — Hide devices without an identified manufacturer

### Signal Strength Filter (Extreme Edition)

Filter by minimum signal strength, from > -10 dBm to > -80 dBm. Useful for finding only nearby devices.

### Text Filters (Extreme Edition)

Search devices by typing part of:

- **Device name** (case-insensitive)
- **MAC address**
- **Vendor name**

A status indicator shows **"Filters on"** or **"Filters off"** with the current device count.

---

## 7. Device Finder

The Device Finder helps you physically locate a Bluetooth device by tracking its signal strength in real time.

### How to Open

Tap a device in the list, then tap the **Find** button.

### Signal Strength Display

- Shows the current RSSI signal strength in dBm (e.g., "-45 dBm")
- Updates continuously as you move closer to or further from the device
- A live graph plots the signal strength over time, so you can see trends

### Play Sound

- Toggle **"Play sound"** to hear an audio tone when the device is detected
- Choose from 5 different sound types using the dropdown
- The sound gets louder as you get closer to the device

### Sound Finder (BLE GATT Audio Devices)

- Toggle **"Enable sound finder"** to make the connected audio device play a loud continuous beep
- This helps locate headphones or earbuds that are connected but out of sight
- **Warning:** This can be very loud — remove headphones from your ears before enabling!
- Only available for audio devices using BLE GATT scanning

### Detection Protocol (Extreme Edition)

Choose which scanning method to use:

- **BLE** — Best for most modern devices (default)
- **BLE GATT** — Active connection mode, enables sound finder for audio devices
- **BR/EDR** — For older Classic Bluetooth devices

If the device is not detected with one protocol, try switching to another.

### Location Tracking (Android 13+)

- Toggle **"Show last known location"** to enable GPS tracking for this device
- See [Section 8](#8-gps-location-tracking-android-13) for full details

### Last Known Location Map

When location tracking is enabled and a position has been recorded:

- A map displays the last known location with a pin marker
- The title shows: **"Last known location (connected/disconnected, date time)"**
- Tap **"Tap to navigate"** to open the location in Google Maps (or another map app)

### Export RSSI Data (Extreme Edition)

Tap the **Export** button to share the signal strength measurements as a CSV file via email, messaging, or other apps.

### Help

Tap the **Help** button for tips on using signal strength to find your device.

### Stopping

Tap **Stop** to end the device finder scan and close the dialog.

---

## 8. GPS Location Tracking (Android 13+)

This feature saves the GPS position of your Bluetooth devices whenever they connect or disconnect. It helps you remember where you last used a device — for example, where you took off your headphones or where your car is parked.

> **Requirement:** Android 13 (API 33) or newer is required. This feature is not available on older Android versions.

### How to Enable

1. Open the **Device Finder** for any device (tap the device, then **Find**)
2. Toggle the **"Show last known location"** switch
3. The app will guide you through the required permissions:
   - **Step 1:** Grant **precise location** permission
   - **Step 2:** Grant **background location** permission — select **"Allow all the time"** when prompted
   - **Step 3:** Confirm the **device association** via the system dialog
4. Once complete, the device is now tracked

### How It Works

- The app uses Android's **Companion Device Manager** to monitor your associated Bluetooth device
- When the device **connects** or **disconnects**, the app automatically records the current GPS location
- This works in the background — you don't need to have the app open
- Locations are stored locally on your device and are never sent anywhere
- Only the most recent location per device is kept (it updates each time the device connects or disconnects)
- If GPS is unavailable at the time of the event, the previous location is kept unchanged

### Viewing the Location

- Open the **Device Finder** for the tracked device
- If a location has been saved, a map will appear showing the last known position
- The title indicates whether the location was recorded on a **connect** or **disconnect** event, along with the date and time
- Tap **"Tap to navigate"** to open the location in Google Maps for turn-by-turn navigation

### After Reboot or App Update

The app automatically re-registers all tracked devices after your phone restarts or after an app update. No action is needed from you — tracking resumes automatically.

---

## 9. History Tab

The History tab stores your past scan sessions so you can review them later.

### Scan Session List

Each entry shows:

- **Date and time** of the scan
- **Total devices** found
- **New devices** count (devices seen for the first time)

### Loading a Session

Tap a session to load its devices into the main device list. This lets you review what was found during that scan.

### Load All (Extreme Edition)

Tap the **Load All** button to combine all history sessions into a single list.

> In the Free edition, only the 2 most recent sessions can be loaded.

### Export CSV (Extreme Edition)

Tap the **Export** button to share your entire scan history as a CSV file.

### Deleting History

- Tap the **Clear** button and confirm to delete all scan history
- Individual sessions can also be deleted

---

## 10. Charts Tab

The Charts tab provides visual statistics about your scanned devices.

### Bar Chart

Shows the number of devices found per scan session over time:

- **All devices** vs **New devices** comparison
- Pinch to zoom, swipe to scroll
- Tap a bar to select that session's data for the pie charts below

### Pie Charts

- **Device group distribution** — Breakdown by category (Computer, Phone, Audio-Video, Wearable, etc.)
- **Vendor distribution** — Top manufacturers found
- **RSSI distribution** — Signal strength breakdown (Amazing, Good, OK, Weak, Bad)

Tap chart segments for detailed values.

> In the Free edition, charts show example data only. The Extreme edition displays your actual scan data.

---

## 11. User-Defined Device Types

You can create custom device types with your own names and images. This is useful when the app doesn't automatically recognize a specific device.

### Creating a Custom Type

1. Open the **Customize** panel for any device
2. In the device type dropdown, scroll to the bottom and select **"User defined..."**
3. Enter a name for your custom type
4. Tap the image area to pick a photo from your gallery
5. Tap **Add** to save

### Setting a Default for Unknown Devices

Toggle **"Use as default for unknown"** on any custom type. Its image will then be shown for all devices the app can't automatically identify.

### Managing Custom Types

- View all your custom types in the list
- Tap a type to edit its name or image
- Delete types you no longer need (they will be removed from all assigned devices)

---

## 12. Settings

Open Settings from the navigation drawer or the overflow menu.

### Extreme Edition Settings

These are only available in the Extreme edition:

- **Restarts scan automatically** — Keeps scanning continuously until you manually stop or close the app
- **Start automatic scan after app launch** — Begins scanning as soon as you open the app

### General Settings

- **Change language** — Choose from 21 languages:
  Default (system), English, Magyar (Hungarian), Portuguese, Русский (Russian), Deutsch (German), Español (Spanish), Italiano (Italian), 日本語 (Japanese), Français (French), Polski (Polish), Nederlands (Dutch), Indo (Indonesian), Türkçe (Turkish), 한국인 (Korean), Svenska (Swedish), Ελληνικά (Greek), Čeština (Czech), Slovenščina (Slovenian), العربية (Arabic), 简体中文 (Chinese Simplified)

- **Change color theme** — Three options:
  - **Dark** — Dark gray theme
  - **Black (AMOLED)** — Pure black theme for AMOLED screens (saves battery)
  - **Flat** — Light theme

- **Show hidden devices** — Reveal devices that were previously marked as "hidden from future search"

- **Enable compact view** — Condensed device list with less detail per item

- **Number of columns (portrait)** — Choose 1, 2, or 3 columns for the device list in portrait mode

- **Number of columns (landscape)** — Choose 1, 2, or 3 columns in landscape mode

- **Force portrait mode** — Locks the screen to portrait orientation (disables rotation)

- **Help in better user experience** — Enable or disable sending anonymous crash and usage data to the developer

> Some settings require an app restart to take effect.

---

## 13. Navigation Drawer

Swipe from the left edge of the screen (or tap the hamburger menu icon) to open the navigation drawer.

### Header

- App name and launcher icon
- Developer name and email
- Edition label (Free or Extreme)
- App version number

### Menu Items

- **Settings** — Opens the Settings screen
- **Change color theme** — Quick access to theme selection
- **Purchase Pro** — View purchase options for the Extreme edition
- **My subscription** — Manage your subscription (only visible if you have an active subscription)
- **EULA** — View the End User License Agreement
- **Privacy policy** — View the data collection and privacy policy

---

## 14. Free vs Extreme Edition

| Feature | Free | Extreme |
|---|:---:|:---:|
| Scan for Bluetooth devices | Yes | Yes |
| View device details (name, type, MAC, RSSI, vendor, services) | Yes | Yes |
| Pair and unpair devices | Yes | Yes |
| Device Finder (signal strength tracking) | Yes | Yes |
| Play sound when device found | Yes | Yes |
| Sound Finder (play beep on audio device) | Yes | Yes |
| GPS location tracking (Android 13+) | Yes | Yes |
| Last known location map and navigation | Yes | Yes |
| Device type group filters | Yes | Yes |
| Date range filter | Yes | Yes |
| Show only new devices filter | Yes | Yes |
| Exclude unknown name/vendor | Yes | Yes |
| Sort by RSSI, name, vendor, address, date, connected | Yes | Yes |
| Reverse sort order | Yes | Yes |
| Change language (21 languages) | Yes | Yes |
| Change color theme (3 themes) | Yes | Yes |
| Compact view and column layout | Yes | Yes |
| Force portrait mode | Yes | Yes |
| Charts (example data only in Free) | Example only | Full data |
| Device customization (rename, type, beep, pin, hide) | Up to 2 devices | Unlimited |
| Signal strength filter (dBm threshold) | No | Yes |
| Text filters (name, MAC, vendor) | No | Yes |
| Detection protocol selector (BLE / BLE GATT / BR/EDR) | No | Yes |
| Auto-restart scan | No | Yes |
| Auto-start scan on app launch | No | Yes |
| Export RSSI data from Device Finder | No | Yes |
| Load all scan history sessions | Last 2 only | All sessions |
| Export scan history as CSV | No | Yes |
| Copy/Share full device info | Limited | Full details |
| Ad-free experience | No (ads shown) | Yes |

### How to Purchase

- Tap **"Purchase Pro"** in the navigation drawer or the About tab
- Choose between:
  - **Subscription** — Auto-renewing with a free trial period
  - **Lifetime license** — One-time purchase, never expires

---

## 15. Tips and Notes

- **Screen stays on during scanning** — The display won't turn off while a scan is running, so you can monitor results without interruption.

- **Bluetooth Adapter Info** — Tap the **"Adapter info"** button at the bottom of the Devices tab to see your phone's Bluetooth capabilities: Bluetooth version, BLE features (2M PHY, Coded PHY, Extended Advertising), multi-advertisement support, LE audio support, and maximum connected devices per profile.

- **Apple device originality detection** — The app can check if Apple devices (like AirPods) appear to be original or potentially counterfeit. If the check passes, you'll see **"It seems to be original (not fake)"** on the device card.

- **Start scan multiple times** — Some devices may not respond to the first scan attempt. Starting the scan multiple times increases the chance of detecting all nearby devices.

- **Bluetooth must be enabled** — If your phone's Bluetooth is off, the app will prompt you to turn it on. The Enable Bluetooth button in the toolbar provides quick access.

- **App rating** — After using the app for a while, you may be asked to rate it on the Google Play Store. Your feedback helps the developer improve the app!

- **About tab** — Visit the About tab to find links to the developer's other apps (WiFi Analyzer, Network Scanner, SD Card Test, WiFi Speed Test), the developer's blog, and social media.

---

*Bluetooth Scanner is developed by Zoltan Pallagi. For questions or feedback, contact pzoleex.info@gmail.com.*
