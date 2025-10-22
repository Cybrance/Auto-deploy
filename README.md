# 🤖 Bot Restart Action

This GitHub Action automatically restarts your bot hosted on **Cybrancee** whenever you push new code to your repository.  
It’s a simple and reliable way to automatically deploy updates, apply fixes, or refresh your bot’s environment.

---

## 🧩 Requirements

Before setting up, you’ll need:

- A **Cybrancee Panel API Key** — get yours from your [Cybrancee Account](https://panel.cybrancee.com/account)
- Your **Server ID**, found in your bot’s dashboard on the Cybrancee panel

---

## ⚙️ Setup

This GitHub Action requires **one secret** and **one variable** to be configured in your repository.

1. Go to your repository’s **Settings → Secrets and variables → Actions**.
2. Add the following:

   - **Secret:**  
     Name — `PTERODACTYL_API_KEY`  
     Value — your Cybrancee Panel API key

   - **Variable:**  
     Name — `SERVER_ID`  
     Value — your Cybrancee server ID

3. After setting them up, navigate to the **Actions** tab and create a new workflow.
4. Paste the contents of [`main.yml`](/main.yml) into your workflow file and commit the changes.

---

## 🔁 Result

Once configured, every time you push to your `main` branch, your bot will:

- Automatically restart on Cybrancee
- Pull the latest changes from your repository
- Stay up to date without manual restarts

---

© 2025 Cybrancee. All rights reserved.
