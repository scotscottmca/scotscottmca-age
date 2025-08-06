# Age Counter Website

A single-page website that displays my current age down to the second, based on birth date: October 10, 1990.

## 🚀 Live Website

Visit the live site at: [Your GitHub Username].github.io/[Repository Name]

## 📁 Project Structure

```
scotscottmca-age/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions deployment workflow
├── assets/
│   └── avatar.png             # Favicon and touch icon
├── .gitignore                 # Git ignore file
├── README.md                  # This file
└── index.html                 # Main website file
```

## ✨ Features

- **Real-time age calculation** updated every second
- **Multiple time units**: years, months, days, hours, minutes, seconds
- **Precise age display** in decimal years (9 decimal places)
- **Responsive design** that works on desktop and mobile
- **Dark theme** matching your blog's aesthetic
- **Smooth animations** and visual effects
- **Custom favicon** using your avatar

## 🔧 Deployment Workflow

This project uses **GitHub Actions** for automatic deployment to GitHub Pages.

### Automatic Deployment
Every time you push to the `main` branch, the website will automatically:
1. Build and validate the content
2. Deploy to GitHub Pages
3. Be available within minutes

### Manual Setup (One Time Only)

1. **Create GitHub Repository**
   ```powershell
   # Initialize git repository
   git init
   git add .
   git commit -m "Initial commit: Age counter website"
   git branch -M main
   
   # Add your GitHub repository (replace with your details)
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Navigate to **Settings** → **Pages**
   - Under **Source**, select **"GitHub Actions"**
   - The workflow will automatically deploy on the next push

3. **Repository Permissions** (if needed)
   - In repository **Settings** → **Actions** → **General**
   - Ensure **"Read and write permissions"** is selected
   - Check **"Allow GitHub Actions to create and approve pull requests"**

## 🛠️ Local Development

To test locally:
```powershell
# Navigate to project directory
cd "/Users/scott/Dev/scotscottmca-age"

# Open in browser (or use VS Code's Live Server extension)
start index.html
```

## 📝 Customization

### Change Birth Date
Edit line ~157 in `index.html`:
```javascript
const birthDate = new Date('1990-10-10T00:00:00');
```

### Update Favicon
Replace `assets/avatar.png` with your preferred icon (32x32px recommended)

### Modify Colors
All colors are defined in the CSS section of `index.html`:
- Background: `#1a1a1a`
- Container: `#2d2d2d`
- Text: `#ffffff`, `#e0e0e0`, `#b0b0b0`
- Sections: `#404040`

## 📊 Deployment Status

The deployment status can be monitored in:
- **Actions tab** of your GitHub repository
- **Environments** section showing deployment history
- **Settings** → **Pages** showing the live URL

## 🔄 Making Updates

Simply push changes to the main branch:
```powershell
git add .
git commit -m "Update: description of changes"
git push
```

The site will automatically redeploy within 2-3 minutes.
