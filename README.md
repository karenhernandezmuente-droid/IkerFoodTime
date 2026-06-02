# 🐱 IkerFoodTime - Cat Feeding Reminder PWA

Never forget to feed Iker again! IkerFoodTime is a Progressive Web App designed to help you manage your cat's feeding schedule with timely reminders and feeding history tracking.

## ✨ Features

- **📲 Installable**: Install directly to your phone's home screen
- **🔔 Smart Notifications**: Get reminders at scheduled feeding times
- **⏰ Flexible Scheduling**: Set custom feeding names and times
- **📅 Repeat Daily**: Option to create recurring daily feeding reminders
- **📋 Feeding History**: Track when Iker was last fed
- **📱 Works Offline**: Full offline support with service worker caching
- **🌐 No Backend Required**: All data stored locally on your device

## 🚀 Getting Started

### Installation Options

#### Option 1: GitHub Pages (Easiest)
1. Fork this repository to your account
2. Go to Settings → Pages
3. Under "Build and deployment", select "Deploy from a branch"
4. Choose the main branch and root folder
5. GitHub will give you a free HTTPS link
6. Open the link on your phone and install!

#### Option 2: Self-Hosted
1. Download or clone these files
2. Upload to any web server with HTTPS
3. Open in your browser and install to home screen

#### Option 3: Local Development
1. Clone the repository
2. Run a local HTTPS server (or use a tool like `http-server`)
3. Open `https://localhost:8000` in your browser

### Phone Setup

**Android:**
- Open the app in Chrome
- Tap the install prompt or use the "Install App" button
- Allow notifications when prompted

**iPhone (iOS 16.4+):**
1. Open the app in Safari
2. Tap the Share button
3. Select "Add to Home Screen"
4. Open the app from your new home screen icon
5. Enable notifications in the app
6. Go to Settings → Notifications → IkerFoodTime → Allow Notifications

## 📖 How to Use

1. **Enable Notifications**: Tap "Enable Notifications" to get reminders
2. **Schedule Feedings**: 
   - Enter a feeding name (e.g., "Breakfast", "Lunch", "Dinner")
   - Select the time of day
   - Choose if it should repeat daily
   - Tap "Add Feeding Schedule"
3. **Get Reminders**: You'll receive notifications at the scheduled times
4. **Track History**: Mark feedings as complete and view the history
5. **Manage Schedules**: Delete or modify feeding schedules as needed

## 🔔 Notification Tips

- **Keep the app installed**: This starter version sends notifications while the app is open
- **True push notifications**: For background notifications (app closed), you would need to integrate Firebase Cloud Messaging or a Web Push service
- **Test mode**: Use short times (like 1 minute from now) to test notifications

## 📱 Browser Support

- ✅ Chrome/Edge (Android)
- ✅ Safari (iOS 16.4+)
- ✅ Firefox
- ✅ Samsung Internet

## 🛠️ Technical Details

### Files
- `index.html` - Main app interface
- `app.js` - Core app logic and reminder scheduling
- `styles.css` - Cat-themed styling
- `sw.js` - Service worker for offline support
- `manifest.webmanifest` - PWA configuration

### Data Storage
- All feeding schedules and history stored in browser's localStorage
- No data sent to external servers
- Data persists even when app is offline

### Service Worker
- Caches all app assets for offline access
- Handles notification clicks
- Ready for push notification integration

## 🐱 Customization

Want to personalize the app? You can edit:
- **App name**: Change in `manifest.webmanifest`
- **Colors**: Update CSS variables in `styles.css` (search for `:root`)
- **Cat name**: Replace "Iker" with your cat's name throughout
- **Icons**: Replace PNG files in `icons/` folder with custom cat icon

## 🚢 Deployment

### Deploy to GitHub Pages
```bash
git push origin main
```
Then enable Pages in your repository settings.

### Deploy to Other Hosts
Upload all files to your web server and ensure HTTPS is enabled.

## 🐛 Troubleshooting

**Notifications not working?**
- Make sure notifications are enabled in the app
- Check browser notification permissions
- Try refreshing the page
- For iOS, ensure you're using Safari 16.4 or later

**App won't install?**
- Make sure you're using HTTPS (required for PWA)
- Try a different browser
- Clear browser cache and cookies

**History not saving?**
- Check browser storage settings (may be limited in private/incognito mode)
- Ensure localStorage is enabled
- Check available storage space on device

## 📄 License

Free to use and modify for personal use. Feel free to fork and customize!

## 💡 Future Ideas

- Background push notifications with Firebase
- Multiple cat support
- Custom feeding amounts and meal types
- Photo reminders
- Feeding statistics and analytics
- Dark mode
- Multiple reminder times per day

---

**Happy feeding! Keep Iker happy and well-fed! 🐱🍖**
