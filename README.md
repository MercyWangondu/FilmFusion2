# 📽️ FilmFusion

## 🎬 Welcome to FilmFusion
FilmFusion is a modern and stylish movie streaming platform that provides users with an immersive viewing experience.

## 🚀 Features
- 🔎 **Search for Movies**: Find your favorite movies instantly.
- 📱 **Responsive Design**: Optimized for all screen sizes.
- 🎨 **Modern UI/UX**: Stylish and visually appealing interface.
- 🎥 **Movie Playback (Coming Soon)**: The movie player feature is still being worked on.

## 🛠️ Technologies Used
- ⚛️ **React.js** - Frontend framework
- 🚏 **React Router** - Navigation
- 🎨 **CSS (Styled Components)** - Modern styling
- 🎬 **MovieDB API** - Fetch movie details

## 📦 Installation
Follow these steps to set up FilmFusion on your local machine:

```sh
# Clone the repository
git clone https://github.com/MercyWangondu/FilmFusion.git

# Navigate to the project directory
cd FilmFusion

# Install dependencies
npm install

# Start the development server
npm start
```

## 🔗 API Integration
FilmFusion fetches movie details from The Movie Database (TMDb). To integrate the API, follow these steps:
Obtain an API key from TMDb by signing up on the website.
In the project, create a services folder and an api.js file in the root directory and add your API key in the variable shown below:

```
const API_KEY = "";
```
## 🎥 How to Use

- Search for a Movie - Use the search bar to find a movie.
- Click to Watch - Select a movie to start streaming.
- Enjoy Seamless Playback - Watch movies with smooth controls (Movie playback feature is still under development).

## 🔗 API Integration  

FilmFusion fetches movie details from **The Movie Database (TMDb)**. To integrate the API, follow these steps:  

 1. Sign up at [TMDb](https://www.themoviedb.org/) and get an API key. 
  
 2. Inside the project, create a `services` folder.  
3. Add an `api.js` file in the root directory.  
4. Add the following code:  

```js
const API_KEY = "your_api_key_here";
```

## 🔥 Firebase Setup  

FilmFusion uses **Firebase** for authentication, storing user profiles, and managing favorites. Follow these steps to set it up:  

### 1️⃣ Create a Firebase Project  
- Go to [Firebase Console](https://console.firebase.google.com/).  
- Click **"Add Project"** and follow the setup process.  
- Enable **Firestore Database** and **Authentication** in the Firebase settings.  

### 2️⃣ Add Firebase to Your React App  
- In your Firebase project, go to **Project Settings > General** and scroll down to **"Your Apps"**.  
- Select **Web App**, register your app, and copy the Firebase config.  

### 3️⃣ Set Up Firebase in Your Project  
1. Create a **`Firebase`** folder in the project.  
2. Inside it, create a **`firebaseconfig.js`** file.  
3. Add your Firebase configuration like this:  

```js
import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";
import { getFirestore } from "firebase/firestore";

const firebaseConfig = {
  apiKey: "YOUR_FIREBASE_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};

const app = initializeApp(firebaseConfig);
export const auth = getAuth(app);
export const db = getFirestore(app);
```
### 4️⃣ Install Firebase in Your Project
Run this command in your terminal:

```js
npm install firebase
```

##  🎥 How to Use

- 🔎 Search for a Movie – Use the search bar to find a movie.
- ❤️ Add to Favorites – Save movies to your favorites.
- 👤 Profile Page – Update name, email, and profile picture.
- 🔑  Register/Login (optional) 



