# Cloud & Firebase Integration for Mobile Apps

## About the Project
I built this **Firebase Chat App** to explore cloud integration in mobile development. It’s a real-time messaging application that uses **Firebase** as a backend-as-a-service (BaaS) to handle user management and data storage. Instead of building a custom server, I connected the app to the cloud to allow users to sign up, log in, and chat instantly.

## Key Features
* **User Authentication**: Users can create secure accounts and log in using their email and password (handled by Firebase Auth).
* **Real-time Messaging**: Messages are synced instantly across devices using Cloud Firestore.
* **Cloud Storage**: All chat history is stored securely in the cloud, so data persists even if the app is closed.
* **Live Updates**: The chat interface updates automatically when a new message arrives without needing to refresh.

## Under the Hood: Firebase Integration
This app relies on two core Firebase services:
1.  **Firebase Authentication**: I used this to manage the sign-in and registration flow. It handles the security of user credentials and session management.
2.  **Cloud Firestore**: This is a NoSQL cloud database where messages are stored. I set up a collection that the app listens to, so whenever a document (message) is added, the UI updates immediately.
