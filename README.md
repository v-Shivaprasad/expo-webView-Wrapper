# Expo WebView Wrapper

This project is an Expo React Native application that wraps a website within a WebView component. It allows you to create a mobile app experience for any web-based content by embedding it in a native mobile application.

## Features

- Wraps any website in a WebView
- Compatible with both iOS and Android devices
- Easy to deploy and customize

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

- **Node.js**: Install Node.js from [https://nodejs.org/](https://nodejs.org/)
- **Expo CLI**: Install Expo CLI globally by running:
  ```bash
  npm install -g expo-cli
  ```

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/expo-webview-wrapper.git
   cd expo-webview-wrapper
   ```

2. **Install Dependencies**

   ```bash
   npm install
   ```

3. **Update WebView URL**
   Open `App.js` and update the WebView URL to the website you want to display in the app:
   ```javascript
   <WebView source={{ uri: "https://your-website-url.com" }} />
   ```

### Running the App

To run the app on your local development environment:

1. Start the Expo development server:

   ```bash
   npx expo start
   ```

2. Scan the QR code displayed in the terminal or browser with the Expo Go app (available on both iOS and Android) to view the app on your physical device.

### Building for Production

To build a standalone APK for Android:

1. **Set up Expo Application Services (EAS)** (only needed if building for the first time).

   ```bash
   npx expo install eas-cli
   eas login
   ```

2. **Build the APK**
   ```bash
   eas build -p android --profile preview
   ```
