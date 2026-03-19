# EarnHub APK Builder

This repo automatically builds an EarnHub APK using GitHub Actions.
No PC, no Android Studio needed.

---

## How to get your APK (Step by Step)

### Step 1 — Create a GitHub account
Go to github.com and sign up if you don't have an account.

### Step 2 — Create a new repository
- Click the "+" icon top right
- Click "New repository"
- Name it: earnhub-apk
- Set it to Public
- Click "Create repository"

### Step 3 — Upload these files
Upload ALL files from this zip maintaining the folder structure:
```
earnhub-apk/
├── .github/
│   └── workflows/
│       └── build.yml
├── www/
│   └── index.html
├── capacitor.config.json
└── package.json
```

To upload:
- Click "uploading an existing file" on your new repo page
- Drag and drop all files
- Click "Commit changes"

### Step 4 — Watch it build
- Click the "Actions" tab in your repo
- You'll see "Build EarnHub APK" running
- Wait about 5–10 minutes for it to finish

### Step 5 — Download your APK
- Click on the completed workflow run
- Scroll down to "Artifacts"
- Click "EarnHub-APK" to download
- Install it on your phone!

---

## Notes
- The app loads earnhubs.netlify.app inside a native Android wrapper
- This is a debug APK — works fine for personal use and testing
- For Play Store release, you'll need a signed APK (ask for instructions)
- Every time you push changes to GitHub, it auto-rebuilds the APK
