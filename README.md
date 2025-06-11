# expense-tracker-public
# 🔍 Lens - Personal Finance Tracker

A Progressive Web App (PWA) for personal expense tracking and budgeting with clear financial insights.

## 🚀 Live Demo

Visit the live app: [Your GitHub Pages URL will go here]

## 📱 Features

- **Progressive Web App**: Install on mobile and desktop devices
- **Offline Support**: Works without internet connection
- **Expense Tracking**: Log one-time and recurring expenses
- **Budget Management**: Set monthly budgets and track spending
- **Smart Insights**: AI-powered spending analysis and recommendations
- **Multiple Currencies**: Support for GBP, EUR, USD, JPY
- **Dark Mode**: Light and dark theme support
- **Data Export/Import**: Backup and restore your financial data

## 🛠️ Setup Instructions for GitHub Pages

### Step 1: Repository Setup

1. **Fork or create a new repository** on GitHub
2. **Clone the repository** to your local machine:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

### Step 2: File Structure

Organize your files like this:
```
your-repo-name/
├── index.html                 # Rename expense-tracker.html to this
├── manifest.json             # PWA manifest
├── sw.js                     # Service worker
├── generate-icons.html       # Icon generator (optional)
├── icons/                    # Icon folder
│   ├── icon-72x72.png
│   ├── icon-96x96.png
│   ├── icon-128x128.png
│   ├── icon-144x144.png
│   ├── icon-152x152.png
│   ├── icon-192x192.png
│   ├── icon-384x384.png
│   └── icon-512x512.png
└── README.md
```

### Step 3: Generate PWA Icons

1. **Open `generate-icons.html`** in your browser
2. **Click "Generate All Icons"**
3. **Download all generated icons**
4. **Create an `icons/` folder** in your repository
5. **Upload all icon files** to the `icons/` folder

### Step 4: Update Manifest for Your Repository

Edit `manifest.json` and update these fields with your repository name:

```json
{
  "start_url": "/your-repo-name/",
  "scope": "/your-repo-name/",
  // ... rest of the manifest
}
```

Replace `your-repo-name` with your actual GitHub repository name.

### Step 5: Update Service Worker

Edit `sw.js` and update the cache paths if needed:

```javascript
const STATIC_FILES = [
  '/your-repo-name/',
  '/your-repo-name/index.html',
  '/your-repo-name/manifest.json',
  // ... other files
];
```

### Step 6: Enable GitHub Pages

1. **Push your changes** to GitHub:
   ```bash
   git add .
   git commit -m "Add PWA support for Lens expense tracker"
   git push origin main
   ```

2. **Go to your repository settings** on GitHub
3. **Navigate to "Pages" section**
4. **Select source**: Deploy from a branch
5. **Select branch**: main (or master)
6. **Select folder**: / (root)
7. **Click "Save"**

### Step 7: Access Your PWA

Your app will be available at:
```
https://yourusername.github.io/your-repo-name/
```

It may take a few minutes for GitHub Pages to deploy your site.

## 📱 Installing the PWA

### On Mobile (Android/iOS):
1. **Open the app** in your mobile browser
2. **Look for "Add to Home Screen"** prompt or
3. **Tap the browser menu** and select "Add to Home Screen"
4. **Follow the prompts** to install

### On Desktop (Chrome/Edge):
1. **Open the app** in your browser
2. **Look for the install icon** in the address bar or
3. **Click the three-dot menu** and select "Install Lens"
4. **Follow the prompts** to install

## 🔧 Development

### Local Development

1. **Clone the repository**
2. **Open `index.html`** in your browser, or
3. **Use a local server** for better PWA testing:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if you have live-server installed)
   npx live-server
   ```

### Testing PWA Features

1. **Test offline functionality**: Disconnect internet and reload
2. **Test installation**: Look for install prompts
3. **Test on mobile**: Use browser dev tools device simulation

### Customization

- **Colors**: Update theme colors in `manifest.json` and CSS variables
- **Icons**: Regenerate icons using `generate-icons.html`
- **Name**: Update app name in `manifest.json` and HTML title
- **Features**: Modify the JavaScript in `index.html`

## 🐛 Troubleshooting

### PWA Not Installing
- Check that `manifest.json` and `sw.js` are accessible
- Verify all required icons are present in the `icons/` folder
- Ensure HTTPS (GitHub Pages provides this automatically)

### Service Worker Issues
- Check browser console for errors
- Update cache names in `sw.js` when making changes
- Clear browser cache and reload

### GitHub Pages Not Working
- Ensure `index.html` exists in the repository root
- Check that repository is public (or you have GitHub Pro for private repos)
- Wait a few minutes for deployment

### Icons Not Loading
- Verify icon files are in the `icons/` folder
- Check that paths in `manifest.json` match your file structure
- Regenerate icons if needed

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature-name`
3. **Make your changes**
4. **Test thoroughly**
5. **Submit a pull request**

## 💡 Feedback

Found a bug or have a feature request? Please [open an issue](https://github.com/yourusername/your-repo-name/issues) on GitHub.

---

**Made with ❤️ for better personal finance management**
