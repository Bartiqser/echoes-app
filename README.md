
# Echoes

Echoes is a music-sharing app designed for artists, producers, and music enthusiasts to showcase their beats, tracks, and sounds. The app provides a platform to share your creations, explore music from others, leave comments, and like your favorite tracks. Built with Firebase, Echoes ensures seamless user interaction, real-time updates, and secure storage for your music.

---

## Features

- **User Authentication**: Secure registration and login using email and password.
- **Share Your Music**: Upload your songs, beats, or audio tracks to share with the community.
- **Interact with Content**:
  - Like tracks to show your appreciation.
  - Comment on tracks to start conversations or provide feedback.
- **Discover Music**: Browse and explore the music shared by other users.
- **Search Functionality**: Quickly find tracks based on keywords like titles or genres.

---

## Technologies Used

- **Android Studio**: Development environment for building the app.
- **Firebase Services**:
  - **Firebase Authentication**: Secure user login and registration.
  - **Firebase Firestore**: Real-time NoSQL database for storing user data, tracks, likes, and comments.
  - **Firebase Storage**: Cloud storage for uploading and managing audio files.
- **Figma**: For designing the app’s user interface.

---

## Setup and Installation

Follow these steps to set up the project:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/echoes.git
   cd echoes
   ```

2. **Set Up Firebase**
   - Go to [Firebase Console](https://console.firebase.google.com/).
   - Create a new Firebase project.
   - Add your app’s package name and download the `google-services.json` file.
   - Place the `google-services.json` file in the `app/` directory of the project.

3. **Add Dependencies**
   Add the following dependencies to your `build.gradle` file:
   ```gradle
   implementation 'com.google.firebase:firebase-auth:22.0.0'
   implementation 'com.google.firebase:firebase-firestore:24.0.0'
   implementation 'com.google.firebase:firebase-storage:20.0.0'
   ```

4. **Run the App**
   - Open the project in Android Studio.
   - Connect an Android device or use an emulator.
   - Click **Run** to start the app.

---

## App Architecture

The app uses the **Model-View-Controller (MVC)** architecture to ensure clean separation of concerns:

### Firestore Collections
1. **Users Collection**
   Stores user details such as username, email, and profile picture.

2. **Tracks Collection**
   Stores information about uploaded tracks, including title, description, file URL, user ID, and timestamp.

3. **Comments Collection**
   Stores user comments on tracks.

4. **Likes Collection**
   Tracks which users liked specific tracks.

---

## Future Enhancements

- Implement filters for browsing tracks by genre or popularity.
- Add a user profile page to showcase individual uploads.

---
