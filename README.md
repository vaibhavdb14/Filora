# Filora

Filora is a **decentralized file sharing and storage system** built using **Firebase** (for authentication and user management) and **IPFS** (via Pinata) for distributed file storage.  
It allows users to upload, manage, and securely share files with other registered users.

---

## Features
- 🔐 **User Authentication** using Firebase  
- ☁️ **Upload & Store Files** on IPFS (via Pinata API)  
- 📤 **Share Files** with other registered users  
- 📂 **Personal Dashboard** for managing uploaded files  
- 📩 **Shared Files Page** to view files received from others  
- 🎨 **Modern UI** with responsive design  

---

## Project Structure
- `index.html` → Login / Registration page  
- `dashboard.html` → User dashboard for uploads & file management  
- `shared.html` → Shared files page  
- `about.html` → About Filora page (optional)  
- `contact.html` → Contact / feedback form  

---

## Setup & Installation
1. **Clone the repository**
   ```bash
   git clone https://github.com/<your-username>/filora.git
   cd filora

2. **Add Firebase configuration**
In your HTML/JS files where Firebase is initialized, replace placeholders with your Firebase credentials:

```bash
const firebaseConfig = {
  apiKey: "YOUR_FIREBASE_API_KEY",
  authDomain: "YOUR_PROJECT.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

3. **Add Pinata API keys**
In the upload section of your dashboard JS:

```bash
xhr.setRequestHeader("pinata_api_key", "YOUR_PINATA_API_KEY");
xhr.setRequestHeader("pinata_secret_api_key", "YOUR_PINATA_SECRET");
```

4. **Open project in browser**
Simply open index.html in any browser.