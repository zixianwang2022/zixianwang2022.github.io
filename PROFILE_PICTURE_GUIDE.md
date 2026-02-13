# 📸 How to Upload Your Profile Picture

## Step 1: Prepare Your Picture
- Save your professional headshot as **`profile.png`** 
- Recommended size: **300×300 pixels** (or close to square)
- File format: PNG, JPG, or GIF

## Step 2: Upload to Images Folder

You have two options:

### Option A: Upload via GitHub Web Interface (Easiest)
1. Go to your repository: https://github.com/zixianwang2022/zixianwang2022.github.io
2. Navigate to the **`images/`** folder
3. Click **"Add file"** → **"Upload files"**
4. Drag and drop your `profile.png` file
5. Click **"Commit changes"**

### Option B: Upload via Terminal/Command Line
```bash
# Navigate to your project
cd /Users/wangzixian/zixianwang2022.github.io

# Copy your picture to the images folder
cp /path/to/your/photo.png images/profile.png

# Commit and push
git add images/profile.png
git commit -m "Add profile picture"
git push
```

## Step 3: It Will Appear Automatically!
- Once uploaded, your picture will appear in the **left sidebar** at the top
- The filename in `_config.yml` is already set to `"profile.png"`
- Wait ~30 seconds after pushing, then refresh your website

## File Path
```
/Users/wangzixian/zixianwang2022.github.io/
└── images/
    └── profile.png  ← Your picture goes here
```

## What Will Show
Your profile picture will appear:
- 📍 At the top of your left sidebar
- 👤 Above your name "Zixian Wang"
- 🖼️ As a 300px avatar image

---

**Need help? The images folder already exists at `/images/` in your repo!**
