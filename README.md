# Firebase Auth
## Google signin
### Setup
Install plugin to your project
```sh
pnpm i firebase
```
And folowing code to your project
```js
// Import the functions you need from the SDKs you need
import { initializeApp } from "firebase/app";
import { getAuth, GoogleAuthProvider } from "firebase/auth";
// TODO: Add SDKs for Firebase products that you want to use
// https://firebase.google.com/docs/web/setup#available-libraries

// Your web app's Firebase configuration
// For Firebase JS SDK v7.20.0 and later, measurementId is optional
const firebaseConfig = {
	apiKey: "AIzaSyBHPvOSAjC_YDmeDSZlQ8JZbbTFORgqU5o",
	authDomain: "test-firebase-auth-kahwork.firebaseapp.com",
	projectId: "test-firebase-auth-kahwork",
	storageBucket: "test-firebase-auth-kahwork.appspot.com",
	messagingSenderId: "645804867421",
	appId: "1:645804867421:web:f87a39ac2d86b39413b2b4",
	measurementId: "G-B5XJ8XVETL"
};

// Initialize Firebase
const app = initializeApp(firebaseConfig);

//Auth
const auth = getAuth(app);
const provider = new GoogleAuthProvider();
