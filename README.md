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
