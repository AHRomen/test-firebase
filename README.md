# Firebase Test Project

This is a simple Firebase test project to experiment with Firebase features such as authentication, Firestore database, and hosting.

## Prerequisites

Before getting started, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (LTS version recommended)
- [Firebase CLI](https://firebase.google.com/docs/cli) (`npm install -g firebase-tools`)
- A [Firebase Project](https://console.firebase.google.com/)

## Setup

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/firebase-test-project.git
   cd firebase-test-project
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Login to Firebase:
   ```sh
   firebase login
   ```
4. Initialize Firebase in the project:
   ```sh
   firebase init
   ```
   - Select the features you want (Firestore, Authentication, Hosting, etc.).
   - Choose the Firebase project you created earlier.

## Development

- To start a local development server:
  ```sh
  firebase serve
  ```
  or (for hosting preview)
  ```sh
  firebase emulators:start
  ```

## Deployment

To deploy your project to Firebase Hosting:
```sh
firebase deploy
```

## Features

- Firebase Authentication (Google, Email/Password, etc.)
- Firestore Database
- Firebase Hosting
- Cloud Functions (optional)

## Configuration

Ensure your `firebaseConfig` object is correctly set up in your project, typically in `firebase-config.js`:
```js
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

## Resources

- [Firebase Documentation](https://firebase.google.com/docs/)
- [Firebase CLI Guide](https://firebase.google.com/docs/cli)

## License

This project is licensed under the MIT License.

