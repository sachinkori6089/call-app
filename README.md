# Online Calling App

## Description
**Online Calling App** is a web-based application that allows users to make video calls and chat easily. Users can join meetings, share screens, and control their microphone and video. This project is built using **React.js**, **Node.js**, and **Firebase**.  

## Features
- Video calls  
- Instant chat  
- Screen sharing  
- User login/register  
- Join meetings with meeting code  
- Microphone and video controls  
- Guest access for demo/testing  

## Tech Stack
- **Frontend:** React.js, HTML, CSS, JavaScript  
- **Backend & Realtime:** Firebase  
- **Hosting:** Netlify  

## Live Website
[Click here to view](https://online-calling-app.netlify.app/)

## GitHub Repository
[Click here](https://github.com/sachinkori6089/call-app.git)

---

## Firebase Setup

1. **Create a Firebase Project**
   - Go to [Firebase Console](https://console.firebase.google.com/)  
   - Click "Add Project" and create a new project  

2. **Add a Web App**
   - In your project dashboard, click "Add App" → Select "Web"  
   - Give your app a name and click "Register App"  

3. **Copy Firebase Config**
   - In your Firebase app settings, you'll find `firebaseConfig`  
   - Example:
     ```javascript
     const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_PROJECT_ID.appspot.com",
       messagingSenderId: "YOUR_SENDER_ID",
       appId: "YOUR_APP_ID"
     };
     ```

4. **Add to React Project**
   - Create `src/firebase.js` file  
   - Install Firebase:
     ```bash
     npm install firebase
     ```
   - Example code:
     ```javascript
     import { initializeApp } from "firebase/app";

     const firebaseConfig = {
       apiKey: "YOUR_API_KEY",
       authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
       projectId: "YOUR_PROJECT_ID",
       storageBucket: "YOUR_PROJECT_ID.appspot.com",
       messagingSenderId: "YOUR_SENDER_ID",
       appId: "YOUR_APP_ID"
     };

     const app = initializeApp(firebaseConfig);
     export default app;
     ```

---

## Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/sachinkori6089/call-app.git
   cd call-app
