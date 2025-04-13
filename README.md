# Hosting a Vue.js Project on Firebase

Follow these steps to create and deploy your Vue.js application using Firebase Hosting.

---

## 🚀 1. Create a Vue Project

```bash
vue create <ProjectName>
```

---

## 🔧 2. Build the Project

```bash
npm run build
```

---

## 🔥 3. Create a Firebase Project

1. Open [Firebase Console](https://console.firebase.google.com/) in Chrome
2. Login with your Google account
3. Click **Add Project**
4. Enter your project name
5. Click **Continue**
6. Follow the prompts and click **Create Project**

---

## 🛠️ 4. Navigate Back to Your Vue Project

Make sure you’re in your project directory before continuing.

---

## 📦 5. Install Firebase Tools

```bash
sudo npm install -g firebase-tools
```

---

## 🔐 6. Login to Firebase

```bash
firebase login
```

A browser window will open. Select your account and allow access.

---

## 🌐 7. Initialize Firebase Hosting

```bash
firebase init hosting
```

- Choose **Use an existing project** (or create a new one)
- Select your Firebase project
- Set **public directory** to: `dist`
- Configure as a **Single Page App**: `No`
- Set up **Automatic Builds and Deploys**: `No`
- Overwrite `index.html`: `No`

Once done, Firebase Hosting will be initialized.

---

## 🚢 8. Deploy to Firebase Hosting

```bash
firebase deploy --only hosting
```

---

## ✅ 9. Your Project is Live!

After deployment, copy the hosting URL:

```text
HOSTING URL: https://<your-project-name>.web.app
```

---

🎉 You’ve successfully hosted your Vue.js app using Firebase!
```
