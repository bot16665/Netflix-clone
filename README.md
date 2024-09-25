# Netflix Clone

This is a Netflix clone built with **React**, featuring a **Firebase login** page for authentication and using the **TMDb API** for fetching movie categories and details.

## Features

- User authentication using Firebase
- Fetch movie data from TMDb API
- Display various categories like trending, popular, top-rated movies
- Responsive design for a seamless user experience
- User login and sign-up functionality

## Prerequisites

Before running this project, ensure you have installed the following:

- **Node.js**: [Download Node.js](https://nodejs.org/en/download/)
- **npm**: Included with Node.js
- **Firebase account**: [Firebase Setup Guide](https://firebase.google.com/docs/web/setup)
- **TMDb API key**: [Get API Key](https://www.themoviedb.org/settings/api)

## Getting Started

Follow these steps to get a copy of the project up and running on your local machine.

### 1. Clone the repository

```bash
git clone https://github.com/your-username/netflix-clone.git
cd netflix-clone
```

### 2. Install dependencies

```bash
npm install
```

### 3. Set up Firebase

1. Go to [Firebase](https://firebase.google.com/), create a new project.
2. Enable **Authentication** and choose **Email/Password** as the sign-in method.
3. Copy your Firebase config object and paste it into your project under a file named `firebase.js`.

Example `firebase.js`:
```javascript
import firebase from 'firebase/app';
import 'firebase/auth';

const firebaseConfig = {
  apiKey: 'YOUR_API_KEY',
  authDomain: 'YOUR_AUTH_DOMAIN',
  projectId: 'YOUR_PROJECT_ID',
  storageBucket: 'YOUR_STORAGE_BUCKET',
  messagingSenderId: 'YOUR_MESSAGING_SENDER_ID',
  appId: 'YOUR_APP_ID',
};

const firebaseApp = firebase.initializeApp(firebaseConfig);
const auth = firebase.auth();

export { auth };
```

### 4. TMDb API Setup

1. Go to [TMDb](https://www.themoviedb.org/), create an account, and get your API key.
2. Create a `.env` file in the root of your project and add your TMDb API key.

Example `.env`:
```bash
REACT_APP_TMDB_API_KEY=YOUR_TMDB_API_KEY
```

### 5. Run the Project

```bash
npm run dev 
```

The application will run on [http://localhost:3000](http://localhost:3000).

## Folder Structure
![Screenshot 2024-09-26 002922](https://github.com/user-attachments/assets/30150352-3978-41ff-bcb6-5abac1f08064)
![Screenshot 2024-09-26 003022](https://github.com/user-attachments/assets/56bd669b-6e0c-4c05-adf9-dbb90a2176ba)


## Technologies Used

- **React**: JavaScript library for building user interfaces
- **Firebase**: Authentication and real-time database
- **TMDb API**: To fetch movie data
- **CSS**: For styling the app

## License

This project is licensed under the MIT License.

---
