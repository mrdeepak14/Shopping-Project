# Shopping-Project
Welcome to the ShopMate login page! This page allows users to securely log in and access the shopping platform using Firebase Authentication (including Google Sign-In or manual username/password login).
Step 1: Clone the Repository
To start using the ShopMate project, clone this repository:


bash
Copy
cd shopmate
Step 2: Set Up Firebase Authentication
Follow these steps to set up Firebase Authentication for your project:

Go to Firebase Console: Open Firebase Console.

Create a New Firebase Project: If you don't already have a project, create a new one.

Add Firebase to Your Web App:

In the Firebase Console, navigate to your project, click on the </> Web icon to add Firebase to your web app.
Copy the Firebase configuration object.
Add Firebase Configuration: In your login.html file, replace the firebaseConfig object with your Firebase credentials:

javascript
Copy
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID"
};
Enable Google Sign-In:
In the Firebase Console, navigate to Authentication > Sign-In Method.
Enable Google Sign-In.
Step 3: Launch the Project
To view and test the ShopMate Login Page:

Open login.html in your preferred web browser.
To test Firebase functionality, you may need to run the page through a local server:
Use VS Code with Live Server or any other method to run the project.
Or, you can start a simple local server using Python:
bash
Copy
python -m http.server
Navigate to http://localhost:8000 in your browser.
Step 4: Manual Login & Google Sign-In
Google Sign-In: Click the Google Sign-In button to authenticate with your Google account.

Manual Login: Use one of the predefined username and password combinations to log in manually. Here are a few combinations you can use:

Username: user1
Password: password1

Username: user2
Password: password2

Username: user3
Password: password3

Step 5: Redirection to ShopMate Website
Once you successfully log in (either manually or via Google), you will be redirected to the ShopMate website.

The redirection will happen to a demo page Demo.html. Make sure this page exists in your project directory.

Features
Google Sign-In: Allows users to log in using their Google account.
Manual Login: Allows users to log in by entering a predefined username and password.
Redirection to ShopMate Site: Once the user successfully logs in, they will be redirected to the ShopMate website (Demo.html).
File Structure
Here’s a brief overview of the files and structure:

bash
Copy
/shopmate
    /login.html      # The main login page
    /Demo.html       # The page users are redirected to after login
    /style.css       # Styling for the login page
    /script.js       # JavaScript to handle Firebase authentication
Additional Features
You can enhance the project further by:

Creating a Sign-Up Page: For new users to register.
Adding Product Listings: Display products and integrate them with Firebase or a backend service.
Styling Improvements: Customize the design according to your branding.
Integrating More Authentication Methods: Besides Google, you can enable other sign-in methods (Facebook, Email/Password, etc.).

