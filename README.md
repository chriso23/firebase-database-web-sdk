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
#### Get the sample code of the web app
1. Get a local copy of the project's repository by opening terminal and running the following command:
    ```bash
    $ git clone https://github.com/chrisoung/web-database-quickstart
    ```
2. [Create a Firebase Project](https://console.firebase.google.com)
3. [Add the Firebase SDKs and initialize Firebase](https://firebase.google.com/docs/web/setup)
      - Enable [Firebase Realtime Database](https://firebase.google.com/products/realtime-database/?authuser=0)
      - Enable [Firebase Authentication](https://firebase.google.com/docs/auth?authuser=0)
4. [Connect and configure Firebase to your web app](https://firebase.google.com/docs/web/setup?authuser=0#register-app)


Run the sample app
---------------
#### To run the sample app locally, use the Firebase CLI. 

1. On the command line, navigate to your project's root directory; then, run the following command to login to Firebase:

    ```bash
    $ firebase login
   ```
 2. Next, run the `use --add` command to select a Firebase project: 
 
    ```bash
    $ firebase use --add
    ``` 
 
3. To run a sample app locally, use the following command to serve over a local port number: 

    ```bash
    $ firebase serve --only hosting
    ```

Support
-------

- [Firebase Support](https://firebase.google.com/support/)

License
-------
© Chris Oung, 2018. [Apache 2.0 License](../LICENSE)
