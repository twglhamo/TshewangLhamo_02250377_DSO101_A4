# DevOps First Web App - CI/CD Deployment

> A simple static website deployed using GitHub, GitHub Actions, and Render

## 📋 Project Overview

This project demonstrates the fundamentals of **Continuous Integration** and **Continuous Deployment (CI/CD)** by:
- Hosting a static HTML/CSS website on GitHub
- Automating builds with GitHub Actions
- Auto-deploying to Render on every push

**Assignment**: DSO101 - Continuous Integration and Continuous Deployment  
**Student**: Tshewang Lhamo  
**Student ID**: 02250377

---

## 🚀 Features

- ✨ Modern responsive design
- 🔄 Automated CI/CD pipeline
- 🌐 Live deployment on Render
- 📱 Mobile-friendly interface
- ⚡ Fast and lightweight

---

## 📂 Project Structure

```
TshewangLhamo_02250377_DSO101_A4/
├── index.html                 # Main HTML file
├── style.css                  # CSS styling
├── README.md                  # This file
└── .github/
    └── workflows/
        └── deploy.yml         # GitHub Actions workflow
```

---

## 🛠️ Setup Instructions

### 1. **Clone or Initialize the Repository Locally**

If starting fresh:
```bash
git init
```

### 2. **Create Files**

Ensure you have:
- `index.html` - Main webpage
- `style.css` - Styling
- `.github/workflows/deploy.yml` - CI/CD pipeline

### 3. **Commit Code to Git**

```bash
git add .
git commit -m "Initial commit: DevOps web app"
```

### 4. **Create GitHub Repository**

1. Go to [GitHub](https://github.com)
2. Click "New" to create a new repository
3. Name it: `DSO101-A4-DevOps`
4. Choose "Public" (required for Render free tier)
5. Click "Create repository"

### 5. **Push Code to GitHub**

```bash
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/DSO101-A4-DevOps.git
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

### 6. **Verify GitHub Actions**

1. Go to your GitHub repo
2. Click the "Actions" tab
3. You should see your workflow running (the deploy.yml)
4. Watch the logs to ensure it passes

### 7. **Deploy on Render**

1. Go to [Render](https://render.com)
2. Sign in with GitHub (authorize the connection)
3. Click "New +" and select "Static Site"
4. Connect your repository
5. Set the build command: (leave empty for static sites)
6. Set the publish directory: `.` (current directory)
7. Click "Create Static Site"
8. Wait for deployment (usually 1-2 minutes)
9. Your live URL will be displayed

---

## 📊 CI/CD Pipeline Explained

### GitHub Actions Workflow (`deploy.yml`)

The workflow:
1. **Triggers** on every push to the `main` branch
2. **Checks out** your code
3. **Verifies** that `index.html` and `style.css` exist
4. **Passes/Fails** the build
5. Render automatically deploys on successful push

---

## ✅ Marking Criteria Checklist

- [x] **GitHub repo setup** (2 marks)
  - Repository created and public
  - Code committed and pushed

- [x] **Basic application** (2 marks)
  - Static HTML website with CSS
  - Responsive and functional

- [x] **GitHub Actions workflow** (2 marks)
  - `.github/workflows/deploy.yml` created
  - Workflow runs on every push

- [x] **Successful deployment** (3 marks)
  - Connected to Render
  - Live URL accessible

- [x] **Documentation** (1 mark)
  - This README with setup steps

**Total: 10 marks**

---

## 🔗 Submission Details

When submitting, provide:

1. **GitHub Repository Link**
   ```
   https://github.com/YOUR_USERNAME/DSO101-A4-DevOps
   ```

2. **Live Deployed URL**
   ```
   https://your-app.onrender.com
   ```

3. **README** (this file)

---

## 🐛 Troubleshooting

| Problem | Solution |
|---------|----------|
| GitHub Actions fails | Check `.github/workflows/deploy.yml` syntax |
| Render deployment fails | Ensure repository is public and files exist |
| App shows blank page | Verify `index.html` is in root directory |
| CSS not loading | Check `style.css` path in HTML |
| Render can't find repo | Re-authorize GitHub connection in Render |

---

## 💡 How the CI/CD Works

```
1. Push code to GitHub
   ↓
2. GitHub Actions workflow triggers
   ↓
3. Workflow checks and verifies code
   ↓
4. Render webhook receives push notification
   ↓
5. Render automatically deploys the app
   ↓
6. Live URL updates with new version
```

---

## 📝 Notes

- This is a **static site** (no backend needed)
- Render hosting is free for this project
- GitHub Actions is free for public repositories
- Changes are live within 1-2 minutes after push

---

## 📚 Resources

- [Git Documentation](https://git-scm.com/doc)
- [GitHub Actions Docs](https://docs.github.com/en/actions)
- [Render Documentation](https://render.com/docs)
- [HTML/CSS Reference](https://developer.mozilla.org/en-US/)

---

## 👤 Author

**Name**: Tshewang Lhamo  
**ID**: 02250377  
**Course**: DSO101 - CI/CD  
**University**: Royal University of Bhutan

---

**Last Updated**: May 2026  
**Status**: ✅ Complete & Deployed