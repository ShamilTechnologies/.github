# Shamil Mobile App

**Shamil** is a mobile app that allows users to discover, subscribe to, and reserve services with ease. Developed in **Flutter** with a **Firebase backend**, it provides users with access to various service-based businesses and NFC integration for secure access. This repository is focused on the development of the **end-user mobile application**.

---

## 🚀 Project Overview

The **Shamil platform** unifies service providers and consumers under a single system. Key features for end users include:

- 🔍 **Service Discovery**: Find nearby service-based businesses (e.g., gyms, wellness centers, events).
- 📅 **Subscription & Reservation**: Subscribe to or reserve services directly through the app.
- 🔑 **NFC Access**: Access services using NFC devices (bracelet, smartwatch, etc.).
- 📱 **Profile Management**: View and manage subscriptions and reservations.

This app uses **Firebase** for authentication, database, and cloud storage.

---

## 🛠️ Key Components

### 1. **Frontend (Flutter)**

- **Language**: Dart
- **Framework**: Flutter (supports Android & iOS)
- **State Management**: Provider (or chosen state management)
- **Backend Integration**: Firebase SDK
- **Testing**: Unit testing via Flutter's `test` package

### 2. **Backend (Firebase)**

- **Authentication**: Firebase Auth (email, phone, Google sign-in)
- **Database**: Firestore (real-time database for users, subscriptions, reservations)
- **Cloud Storage**: Firebase Storage (stores user documents like payment proofs)
- **Cloud Functions**: Server-side logic (notifications, validation, security)

### 3. **Real-time Services**

- **NFC Integration**: NFC technology verifies active subscriptions or reservations.
- **Push Notifications**: Firebase Cloud Messaging (FCM) for real-time updates.

---

## ⚙️ Development Setup

### Prerequisites

Ensure you have the following installed:

- **Flutter SDK**: [Flutter installation guide](https://flutter.dev/docs/get-started/install)
- **Firebase CLI**: [Firebase CLI installation guide](https://firebase.google.com/docs/cli)
- **Android Studio or Xcode**: For running the app on emulators or devices

### Firebase Configuration

1. Create a Firebase project via the [Firebase Console](https://console.firebase.google.com/).
2. Set up Firebase services (Auth, Firestore, Storage, Cloud Messaging).
3. Download the configuration files:
   - `google-services.json` (Android: place in `android/app/`).
   - `GoogleService-Info.plist` (iOS: place in `ios/Runner/`).
4. Add your Firebase keys to the `.env` file:
   ```bash
   FIREBASE_API_KEY=your_firebase_api_key
   FIREBASE_AUTH_DOMAIN=your_project_auth_domain
   FIREBASE_PROJECT_ID=your_firebase_project_id
