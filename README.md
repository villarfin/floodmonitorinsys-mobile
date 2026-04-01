# Flood Monitoring System Mobile

Separate mobile project for the Flood Monitoring System UI adaptation. This app is built with Expo and React Native.

## Project Overview

This mobile app currently includes these main screens:

- `Dashboard`
- `Monitoring`
- `IncidentReport`
- `Notifications`

Reusable UI components used across the app:

- `MobileCard`
- `StatusBadge`
- `StatsCard`
- `WaterLevelCard`
- `AlertCard`
- `WeatherPanel`

## Files Already Included In This Project

You do not need to create these files manually because they are already part of the repository:

- `package.json` - project dependencies and scripts
- `package-lock.json` - locked dependency versions
- `app.json` - Expo app configuration
- `App.tsx` - app entry point
- `babel.config.js` - Babel configuration
- `tsconfig.json` - TypeScript configuration
- `src/` - source code for screens, components, hooks, styles, and data
- `assets/` - images used by the app

## Prerequisites

Install these tools first on your machine:

1. `Node.js` LTS
2. `npm` (usually installed with Node.js)
3. `Expo Go` on your Android phone if you want to test on a real device
4. One of the following for running locally:
   - Android Studio with an Android emulator
   - Xcode with an iOS simulator if you are on macOS
   - A web browser for Expo web preview

Recommended:

- Use a recent LTS version of Node.js such as Node 20
- Keep Android Studio, Expo Go, and device emulators updated

## How To Run The System

### 1. Open the project folder

Use a terminal and go to the project directory:

```bash
cd floodmonitoringsys-mobile
```

### 2. Install the required packages

Run this command to install all dependencies listed in `package.json`:

```bash
npm install
```

This installs the libraries needed by the app, including:

- `expo`
- `react`
- `react-native`
- `@react-navigation/native`
- `@react-navigation/native-stack`
- `react-native-gesture-handler`
- `react-native-safe-area-context`
- `react-native-screens`
- `typescript`

### 3. Start the Expo development server

Run:

```bash
npm start
```

This starts the Expo server and shows a QR code in the terminal.

## How To Open The App

After `npm start`, choose one of the following:

### Option A: Run on an Android phone using Expo Go

1. Install `Expo Go` from the Google Play Store.
2. Make sure your phone and computer are connected to the same network.
3. Scan the QR code shown in the terminal.
4. The app will open in Expo Go.

### Option B: Run on an Android emulator

1. Open Android Studio.
2. Start an Android emulator.
3. In the terminal where Expo is running, press `a`.

You can also use:

```bash
npm run android
```

### Option C: Run on an iOS simulator

This works only on macOS with Xcode installed.

1. Start the Expo server:

```bash
npm start
```

2. In the terminal, press `i`.

Or run:

```bash
npm run ios
```

### Option D: Run in a web browser

Use:

```bash
npm run web
```

## Important Notes

- No `.env` file is required for the current version of this project.
- No separate backend setup is included in this repository.
- Internet access is recommended because the app fetches weather data from Open-Meteo.
- If `node_modules/` is missing, run `npm install` again.

## Common Commands

```bash
npm install
npm start
npm run android
npm run ios
npm run web
```

## Troubleshooting

### If dependencies fail to install

Try deleting `node_modules` and reinstalling:

```bash
npm install
```

### If Expo does not start correctly

Try clearing the Expo cache:

```bash
npx expo start --clear
```

### If the QR code does not work

- Make sure the phone and computer are on the same Wi-Fi network
- Restart Expo Go
- Restart the Expo server

## Folder Structure

```text
floodmonitoringsys-mobile/
|-- assets/
|-- src/
|   |-- components/
|   |-- data/
|   |-- hooks/
|   |-- navigation/
|   |-- screens/
|   |-- styles/
|   `-- utils/
|-- App.tsx
|-- app.json
|-- babel.config.js
|-- package.json
|-- package-lock.json
`-- tsconfig.json
```

