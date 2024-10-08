# Rakshya - A friend in need

![App ScreenShot](https://i.postimg.cc/3JfvQ0PR/appLogo.jpg)

Welcome to the **Rakshya** – your lifeline in critical situations. This app is your indispensable companion, providing vital first aid information and powerful features to guide you through emergencies with confidence. Offering complete voice control, offline functionality, and location tracking, it's your trusted ally when every moment counts.

## Table of Contents

- [Rakshya - A friend in need](#rakshya---a-friend-in-need)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
    - [🌐 Seamless Offline Capability](#-seamless-offline-capability)
    - [🎙️ Intuitive Voice Control](#️-intuitive-voice-control)
    - [📍 Precision Location Tracking](#-precision-location-tracking)
    - [🚑 Comprehensive First Aid Guidance](#-comprehensive-first-aid-guidance)
    - [🆘 Emergency SOS](#-emergency-sos)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Offline Capability](#offline-capability)
  - [Voice Control](#voice-control)
  - [Location Tracking](#location-tracking)
  - [First Aid](#first-aid)
  - [Emergency SOS](#emergency-sos)

## Features

### 🌐 Seamless Offline Capability

- Enjoy full app functionality even without an internet connection.
- Access vital first aid, location information wherever you are, regardless of connectivity.

### 🎙️ Intuitive Voice Control

- Navigate the app effortlessly using natural voice commands.
- Simply ask for first aid guidance, and our app will provide the answers you seek.

### 📍 Precision Location Tracking

- Benefit from offline location tracking to pinpoint your exact coordinates.
- In emergencies, your location is at your fingertips, even when you're offline.

### 🚑 Comprehensive First Aid Guidance

- Access expert step-by-step first aid instructions for a wide range of accidents and medical emergencies.
- Quickly find the information you need to respond effectively to common injuries, burns, fractures, and more.

### 🆘 Emergency SOS

- Activate the SOS feature to send distress signals and your location to predefined contacts.
- Ensure that help arrives promptly when you need it most.

## Installation

In order to install "Rakshya" in your android device go to [Releases](https://github.com/ptdatta/Rakshya/releases) section of this repository and download the appropriate .apk file according to your device specifications.

If you want to run the app in your local machine, first install all the dependencies required for react native and then follow the instructions below:

```bash
npx react-native@latest init YourProject
```

For Android,

```bash
npx react-native run-android
```

For IOS,

```bash
npx react-native run-ios
```

## Usage

- Allow all the permissions asked during setup for the app to work as intended. (Set location to Allowed all the time)
- Restart the app once after the initial setup.
- Double tap on screen to activate voice mode in home screen.
- Voice commands at [Commands](https://github.com/ptdatta/Rakshya/blob/v1.0.0/voicecommands.md).
- Double tap on the navbar to activate voice mode on other pages than home screen.
- Jerk the phone once to activate panic mode.
- Enjoy your safety.

## Offline Capability

One of the main motivations of making this app was making it accessible to most people at most places. That's why we opted to make this app available fully offline. To make this feature possible we used many native modules instead of libraries as most of them use cloud based functionality for the most part. We wrote modules for speech recognition, text-to-speech, shake detection etc. We even went out of our way to make it possible to track your location without an internet connection.

## Voice Control

As stated earlier to make this app accessible to most people we implemented voice control functionality for the people who don't have the perfect vision. Every gesture that can be handled with touch also has a voice command for it. For reading all the voice commands go to [Voice Commands](https://github.com/ptdatta/Rakshya/blob/v1.0.0/voicecommands.md).

## Location Tracking

For offline location tracking we use the GPS of the phone to get the current longitude and latitude of the user and using various algorithms we tend to use that info in various places throughout our app like showing the user the closed hospitals/medicals to them with contact info and directions.

Note: To get directions to the health centres nearby while offline download the offline Google Maps of your local area.

## First Aid

We researched the web for the most common accidents that require first aid, we scraped the aid for those accidents and converted them in a more user-friendly format in order to provide the users the best experience in their difficult times. We have the aid for accidents ranging from bee stings all the way to life threatening incidents like heart attack.

## Emergency SOS

With just a slight jerk to your app, it activates the panic mode and your current location with an SOS message to your pre defined contacts that are asked to you during the initial setup.
