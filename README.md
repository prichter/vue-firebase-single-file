# vue-firebase-single-file
A single html file for rapid development with vuejs frontend and firebase datastore backend.

# Purpose
This is designed to assist with quick prototyping of an app / page from one html file with no tooling required.  All libraries are loaded via CDN to allow for quick updating or speicfying particular versions.

# Testing
This has not been fully tested for functionality or for security.  Use at your own risk.

# Firebase setup.
This assumes a Firebase account and firestore database has been set up with a 'tasks' collection, with some tasks as shown in the image below:
![Database Tasks Example](/doc/database-tasks-example.png)
An external file is used for firebase credentials in order to allow for CDN publishing.  These can be directly substituted as desired with your own credentials.
The external file is called firebaseConfig.js, and is as follows:
```
const firebaseConfig = {
  apiKey: "YOUR-API-KEY",
  authDomain: "YOUR-AUTH-DOMAIN.firebaseapp.com",
  databaseURL: "YOUR-DATABASE-DETAILS.firebaseio.com",
  projectId: "YOUR-PROJECT-ID",
  storageBucket: "YOUR-STORAGE-BUCKET.appspot.com",
  messagingSenderId: "YOUR-MESSAGING-SENDER-ID",
  appId: "YOUR-APP-ID"
};

export default firebaseConfig;
```
