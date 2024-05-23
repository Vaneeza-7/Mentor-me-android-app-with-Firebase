# MentorMe App with Firebase

This repository contains the source code for the MentorMe app built on Android which utilizes Firebase for backend services. This app was developed as part of the CS4039 Software for Mobile Devices course. 

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Firebase Integration](#firebase-integration)
- [Android Implementation](#android-implementation)
- [Getting Started](#getting-started)
- [Testing](#testing)
- [License](#license)

## Overview
MentorMe is a mobile application designed to connect users with mentors. It features user authentication, mentor management, push notifications, chat functionality, and more. The backend services are powered by Firebase.

## Features
1. **User Authentication:** Sign up, login, and logout functionalities using Firebase Authentication.
2. **Mentor Management:** Add mentors to the list and favorites.
3. **Push Notifications:** For new messages, mentor updates, and other important events using Firebase Cloud Messaging.
4. **Real-time Database:** Stores messages, bookings, and mentor information using Firebase Realtime Database.
5. **Storage:** Securely stores images and other files using Firebase Storage.
6. **Chat System:** Includes text messages, voice notes, image, video, and file uploads.
7. **Camera Integration:** Take and upload photos within chats.
8. **Video/Audio Calls:** Uses Agora API for making calls.
9. **Offline Mode:** App functions properly offline with Firebase Realtime Database.

## Firebase Integration
### Authentication
- **Firebase Authentication** is used for user sign up, login, and logout functionalities.
- **Email/Password Authentication** is implemented for user management.

### Realtime Database
- **Firebase Realtime Database** stores user profiles, mentor details, messages, and booking information.
- Real-time updates ensure that users have the latest information and chat messages.

### Storage
- **Firebase Storage** is used for storing profile pictures, chat images, and other files.
- Ensures secure and scalable storage for user-generated content.

### Cloud Messaging
- **Firebase Cloud Messaging (FCM)** is used to send push notifications for new messages, mentor updates, and other events.
- Notifications are also displayed within the app's notification screen.

## Android Implementation
### Splash Screen
- Displays for 5 seconds before navigating to the next screen.

### User Interface
- **Profile Screen:** Allows users to update their profile picture, cover photo, and personal information.
- **Home Screen:** Displays a list of mentors for easy access.
- **Chat Screen:** Supports text, image, video, and file sharing in real-time.

### Libraries Used
- **Glide:** For image caching and loading, ensuring offline accessibility.
- **Agora SDK:** For implementing video and audio call functionalities.
- **hbb20/Android Country Picker:** For selecting from list of all countries in the world with search functionality.
- **applandeo/Material Calendar View:** For customizable material calendar with range date picker.

### Key Functionalities
- **Search with Filters:** Helps users find mentors based on specific criteria.
- **Session Booking:** Allows users to book sessions with mentors.
- **Favorites:** Users can add mentors to their favorites for quick access.
- **Reviews:** Users can review mentors based on their experiences.
- **Notification of Screenshot:** Notifies users when a chat screenshot is taken.

## Getting Started

### Prerequisites
- Android Studio Hedgehog or latest version.
- Firebase project set up.
- Agora API credentials.

### Installation
1. **Clone the repository:**
    ```sh
    git clone https://github.com/Vaneeza-7/Mentor-me-android-app-with-Firebase.git
    ```
2. **Open the project in Android Studio.**
3. **Connect to Firebase:**
    - Add your `google-services.json` file to the app directory.
    - Configure Firebase in your project settings.
4. **Add Agora API credentials:**
    - Follow the Agora API documentation to set up your credentials.

### Running the App
- Open the project in Android Studio and run the app on an emulator or physical device.

## Testing
- The project includes 3 Espresso test cases to validate key functionalities.
- To run the tests:
    ```sh
    ./gradlew connectedAndroidTest
    ```
    
## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
