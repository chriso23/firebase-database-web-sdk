Firebase Realtime Database Web Quickstart
-----------------------------------------

Introduction
------------
This quickstart sample application demonstrates how to use the Firebase JavaScript SDK and the Firebase Realtime Database to build and deploy a simple social blogging app for the web.

Installation
------------
#### Install the Firebase CLI

The Firebase CLI requires [Node.js](http://nodejs.org/) and [npm](https://npmjs.org/) (the Node Package Manager).

  1. Install Node.js for your computer's operating system. Installing Node.js automatically installs npm.
        - For macOS/Linux, use [nvm](https://github.com/nvm-sh/nvm/blob/master/README.md) (the Node Version Manager)
        - For Windows, use [nvm-windows](https://github.com/coreybutler/nvm-windows).

      **Note**: The Firebase CLI requires Node.js v6.0.0 or later. Some Firebase services might require specific versions of Node.js, so check each Firebase service's getting started page for any specific Node.js requirements.

  2. Install the Firebase CLI using npm by running the following command:

      ```bash
      $ npm install -g firebase-tools
      ```

      This command installs the globally available `firebase` command. To update to the latest version of the Firebase CLI, re-run the same `npm install` command.

Setup
-----
#### Get the sample code from GitHub
1. To get the sample code from GitHub, use the `git clone` command to get a local copy of the remote repository. To clone the sample code, run the following command:

    ```bash
    $ git clone https://github.com/chrisoung/web-database-quickstart
    ```
    
2. [Create a Firebase Project](https://console.firebase.google.com) in the Firebase console.
3. Connect and configure Firebase to your web app.
4. Add the Firebase SDKs and initialize Firebase.
      - Enable [Firebase Realtime Database](https://firebase.google.com/products/realtime-database/?authuser=0).
      - Enable [Firebase Authentication](https://firebase.google.com/docs/auth?authuser=0).

Usage
-----

1. To add Firebase SDKs (Firebase Realtime Database and Authentication) to your web app, select the SDKs as scripts to the bottom of your `<body>` tag. For more information about the supported Firebase SDKs, see [Additional Firebase JS SDKs](https://firebase.google.com/docs/web/setup?authuser=0#available-libraries).
  
    ```javascript
        <!-- The core Firebase JS SDK is always required and must be listed first -->
        <script src="/__/firebase/5.5.7/firebase-app.js"></script>
        <script src="/__/firebase/5.5.7/firebase-auth.js"></script>
        <script src="/__/firebase/5.5.7/firebase-database.js"></script>

        <!-- TODO: Add SDKs for Firebase products that you want to use
        https://firebase.google.com/docs/web/setup#reserved-urls -->

        <!-- Initialize Firebase -->
        <script src="/__/firebase/init.js"></script>
    ```

2. Initialize Firebase in your web app

    ```html
    <body>
        <!-- Previously loaded Firebase SDKs -->

        <script>
        // TODO: Replace the following with your app's Firebase project configuration
        var firebaseConfig = {
        // ...
        };

    // Initialize Firebase
    firebase.initializeApp(firebaseConfig);
        </script>
    </body>
    ```

Run the sample app
---------------
#### To run the sample app locally, use the Firebase CLI and deploy to Firebase Hosting

1. On the command line, navigate to your project's root directory; then, run the following command to login to Firebase:

    ```bash
    $ firebase login
   ```
   This command connects your local machine to Firebase and grants you access to your Firebase projects.

2. [Initialize your Firebase project](https://firebase.google.com/docs/hosting/quickstart?authuser=0#initialize). Run the following command from the root of your local app directory:
    ```bash
    $ firebase init
    ```
    This initialization command does all of the following:
    - Links your local app directory with Firebase.
    - Generates a firebase.json file (a required file for Firebase Hosting).
    - Prompts you to specify a public root directory which contains your public static files (HTML, CSS, JS, etc.).

    The default name for the directory that Firebase looks for is "public". You can also set the public directory later by directly modifying your firebase.json file. 


3. Next, run the `use --add` command to select a Firebase project: 
 
    ```bash
    $ firebase use --add
    ``` 
 
4. To run a sample app locally, use the following command to serve over a local port number: 

    ```bash
    $ firebase serve --only hosting
    ```

Support
-------

- [Firebase Support](https://firebase.google.com/support/)

License
-------
© Chris Oung, 2018. [Apache 2.0 License](../LICENSE)
