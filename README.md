# 🎲 Dungeons of Dumbassery - Card Creator

A web-based tool for creating and managing cards for the Dungeons of Dumbassery card game. Connected to Google Sheets for seamless card management.

![Version](https://img.shields.io/badge/version-2.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## ✨ Features

- ✏️ **Create Cards** - Build new cards with smart form fields that adapt to card type
- 📋 **View Cards** - Browse and filter your existing cards from Google Sheets
- 📖 **Reference** - Complete game rules and card type explanations
- ⚙️ **Settings** - Easy Google Sheets API connection
- 🎨 **Auto-formatting** - Automatically applies bold/italic formatting
- 💾 **Live Preview** - See your card as you create it
- 🔄 **Two View Modes** - Grid view or Table view for your cards

## 🚀 Deployment Instructions

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in (or create account)
2. Click the **"+"** button (top right) → **"New repository"**
3. Repository settings:
   - **Name:** `dod-card-creator` (or any name you like)
   - **Visibility:** Public ✅
   - **Add README:** ✅ Check this box
4. Click **"Create repository"**

### Step 2: Upload Files

1. In your new repository, click **"Add file"** → **"Upload files"**
2. Drag these files into the upload area:
   - `index.html` (the card creator webapp)
   - `README.md` (this file - optional but recommended)
3. Scroll down and click **"Commit changes"**

### Step 3: Enable GitHub Pages

1. Go to your repository's **Settings** tab
2. In the left sidebar, click **"Pages"**
3. Under **"Source"**, select:
   - Branch: **main** (or **master**)
   - Folder: **/ (root)**
4. Click **"Save"**
5. Wait ~1-2 minutes for deployment

### Step 4: Access Your App! 🎉

Your app will be available at:
```
https://YOUR-USERNAME.github.io/dod-card-creator/
```

**Example:** If your GitHub username is `johndoe`, your URL is:
```
https://johndoe.github.io/dod-card-creator/
```

GitHub will show you the exact URL on the Pages settings page.

---

## ⚙️ Google Sheets Setup

To connect the app to your Google Sheets:

### 1. Enable Google Sheets API

1. Go to [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project (or select existing)
3. Navigate to **"APIs & Services"** → **"Library"**
4. Search for **"Google Sheets API"** and enable it

### 2. Create API Key

1. Go to **"Credentials"** → **"Create Credentials"** → **"API Key"**
2. Copy your API key (looks like: `AIzaSyB...`)
3. *(Recommended)* Click **"Restrict Key"**:
   - Application restrictions: **HTTP referrers**
   - Add: `https://YOUR-USERNAME.github.io/*`
   - API restrictions: **Google Sheets API** only

### 3. Get Spreadsheet ID

1. Open your Google Sheet
2. Look at the URL in your browser:
   ```
   https://docs.google.com/spreadsheets/d/1BxiMVs0XRA5nFMdKvBdBZjgmU.../edit
   ```
3. Copy the ID part (between `/d/` and `/edit`)

### 4. Share Your Sheet

1. Click **"Share"** button in your Google Sheet
2. Change to: **"Anyone with the link can VIEW"** ✅
3. Click **"Done"**

### 5. Configure the App

1. Open your deployed app
2. Go to **⚙️ Settings** tab
3. Paste your **API Key**
4. Paste your **Spreadsheet ID**
5. Click **"💾 Save Settings"**
6. Click **"🔍 Test Connection"** to verify

---

## 📋 Card Types Supported

| Card Type | Description |
|-----------|-------------|
| **Classes** | Character foundations with base abilities and dice |
| **Subclasses** | Special twists that combine with Classes for Signature Moves |
| **Stuff & Thangs** | Actions, gear, and spells (mixed deck) |
| **Dungeons** | Challenges with 4 subtypes (Combat, Social, Exploration, Wild) |
| **Creeps** | Chaos Master monsters that compete against the Party |
| **Curses** | Instant chaos effects from the Chaos Master |
| **Casualties** | Random wild events with roll-table mechanics |

---

## 🔄 Updating Your App

When you want to update the app with a new version:

1. Go to your GitHub repository
2. Click on `index.html`
3. Click the **pencil icon** (Edit)
4. Paste the new HTML code
5. Scroll down and click **"Commit changes"**
6. Wait ~30 seconds, then refresh your app URL

---

## 📱 Mobile Friendly

The app is fully responsive and works great on:
- 💻 Desktop browsers
- 📱 Mobile phones
- 📲 Tablets

---

## 🛠️ Troubleshooting

### "Not connected to Google Sheets"
- ✅ Check you've completed all setup steps above
- ✅ Make sure your sheet is shared (Anyone with link can VIEW)
- ✅ Verify API Key restrictions allow your GitHub Pages URL
- ✅ Check browser console (F12) for specific errors

### "Can't save cards"
- ✅ Your sheet must be **publicly editable** OR use OAuth (current version uses API key, which is read-only)
- ✅ For write access, you'll need to make sheet "Anyone with link can EDIT"

### Cards not loading
- ✅ Check your Spreadsheet ID is correct
- ✅ Verify sheet names match exactly: `Classes`, `Subclasses`, `StuffThangs`, `Dungeons`, `Creeps`, `Curses`, `Casualties`
- ✅ Ensure first row has column headers

---

## 🎮 How to Use

1. **Go to Settings** → Enter API credentials → Save
2. **Create Card Tab** → Select card type → Fill fields → Save
3. **View Cards Tab** → Browse/filter your cards → Refresh as needed
4. **Reference Tab** → Check game rules anytime

---

## 📄 License

MIT License - Feel free to use, modify, and share!

---

## 🎲 About Dungeons of Dumbassery

A simplified, humor-filled card game that captures the spirit of D&D with Cards Against Humanity irreverence and Munchkin-style chaos.

**Game Designer:** [Your Name]  
**Version:** 3.2  
**Tool Version:** 2.0

---

## 💡 Tips

- **Bookmark your app URL** for quick access
- **Settings are saved** in your browser (localStorage)
- **CSV Export** works offline - copy and paste into sheets manually if needed
- **Print-friendly** - Use browser print for card lists

---

## 🆘 Need Help?

If you encounter issues:
1. Check the Troubleshooting section above
2. Open browser console (F12) to see error messages
3. Verify all Google Sheets setup steps were completed
4. Make sure your sheet structure matches the expected format

---

**Happy Card Creating! 🎲✨**
