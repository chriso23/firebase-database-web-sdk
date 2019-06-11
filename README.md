Firebase Realtime Database Web Quickstart
-----------------------------------------
The Firebase Realtime Database lets you store and sync data between users and devices in real-time by using a cloud-hosted, NoSQL database. All updated data syncs across connected client devices in milliseconds, and data remains available if your app goes offline, which provides a great user experience regardless of network connectivity.

Introduction
------------
This quickstart sample app contains a step-by-step guide that demonstrates how to connect your web application to Firebase, set up the Firebase Realtime Database Web SDK, and configure the database rules to build a simple blogging application that allows authorized users to post and retrieve data in real-time.

[Read more about the Firebase Realtime Database](https://firebase.google.com/docs/database/)

Getting Started
---------------

 1. Create your project on the [Firebase Console](https://console.firebase.google.com).
 1. Enable the **Google** sign-in provider in the **Authentication > SIGN-IN METHOD** tab.
 1. You must have the Firebase CLI installed. If you don't have it install it with `npm install -g firebase-tools` and then configure it with `firebase login`.
 1. On the command line run `firebase use --add` and select the Firebase project you have created.
 1. On the command line run `firebase serve` using the Firebase CLI tool to launch a local server.


License
-------

© Chris Oung, 2018. [Apache 2.0 License.](https://github.com/chrisoung/firebase-realtime-database/blob/master/LICENSE)
