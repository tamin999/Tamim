# 🐐 Goat Bot v2

A **Messenger Bot** built using **Node.js** that runs on your personal Facebook account.  
Made with ❤️ by **NTKhang** & customized for extended use.

---

## ✨ Features

- 📌 Auto-restart & crash recovery  
- 🛠 Easy-to-use command system  
- 🔒 Role-based permissions (admin/user)  
- ⚡ Fast & lightweight with Node.js v20  
- 📝 Configurable `config.json` for quick setup  
- 🌐 Multi-language support  

---

## 1️⃣ Config Setup

Before running the bot, set your **command prefix** and **admin user ID** in `config.json`.

```json
{
  "prefix": "#",                    // Your command prefix
  "admin": ["YOUR_ADMIN_ID"],       // Your Facebook user ID
  "botName": "Goat Bot v2",
  "autoRestart": true,
  "language": "en",
  "fbState": []                     // Facebook appState (cookies) will go here
}

> Tip: Replace "YOUR_ADMIN_ID" with your Facebook user ID, and "#" with your preferred command prefix.




---

2️⃣ Facebook Account Setup

You need to provide your Facebook cookies / appState for the bot to login.

Steps:

1. Open your Facebook account on Chrome or any browser.


2. Extract appState using tools like fb-chat-api or Chrome extensions.


3. Paste it into config.json under "fbState".



> ⚠️ Keep this information private. Do not share publicly.




---

3️⃣ Run on Render 🚀

You can host Goat Bot v2 on Render using your config.json.

Steps:

1. Push your bot repository to GitHub.


2. Ensure the following files are included:

index.js

package.json

config.json



3. Update package.json:



{
  "name": "goat-bot-v2",
  "version": "1.0.0",
  "main": "index.js",
  "scripts": {
    "start": "node index.js"
  },
  "engines": {
    "node": "20.x"
  },
  "dependencies": {
    "fb-chat-api": "^1.0.0"
  }
}

4. Render Setup:

Dashboard → New + → Web Service

Connect your GitHub repo

Select Node.js environment

Build Command:


npm install

Start Command:


npm start


5. Deploy ✅



Keep Bot Running

Free Render plan may sleep when idle.

Options to keep bot alive:

Use UptimeRobot or Cron-job.org to ping every 5 minutes

Upgrade to a paid plan for 24/7 uptime




---

4️⃣ Personal Info 🧑‍💻

Facebook: www.Facebook.com/arafatas602

https://i.postimg.cc/k42DBr6X/510782721-1448006386615670-6777572953755986867-n.jpg

---

⚠️ Disclaimer

This bot is for educational purposes only.
Do not misuse it.
The author is not responsible for any problems arising from misuse.
