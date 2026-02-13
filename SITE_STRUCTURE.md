# Your Site Structure Explained

## Three Main Files Control Your Website

### 1️⃣ `_config.yml` (Controls Sidebar)
**Location:** `/Users/wangzixian/zixianwang2022.github.io/_config.yml`

This file controls what appears in the **LEFT SIDEBAR** of your website.

**What you see on the website:**
```
┌─────────────────┐
│ [PHOTO]         │ ← avatar field
│                 │
│ Zixian Wang     │ ← author.name field
│                 │
│ He/Him          │ ← author.pronouns field
│                 │
│ First-year PhD  │ ← author.bio field
│ student at UIUC │
│ advised by...   │
│                 │
│ 📧 Email icon   │ ← author.email creates link
│ 🐙 GitHub icon  │ ← author.github creates link
│ etc.            │ ← all profile URLs
└─────────────────┘
```

**What you're updating:**
- `author.name` = Your name on sidebar ✅ Set to "Zixian Wang"
- `author.bio` = Short description ✅ Set to PhD student bio
- `author.pronouns` = ✅ Already "He/Him"
- `author.email` = ✅ Already "zixianw4@illinois.edu"
- `author.avatar` = Profile picture filename ⏳ Needs image file

**Still TODO in _config.yml:**
- All the academic profile URLs (Google Scholar, arXiv, ORCID, etc.) - leave blank if you don't have them

---

### 2️⃣ `_pages/about.md` (Controls Main Content)
**Location:** `/Users/wangzixian/zixianwang2022.github.io/_pages/about.md`

This file controls what appears in the **CENTER/MAIN AREA** of your website.

**What you see on the website:**
```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
Welcome to My Academic Portfolio

About Me
I am a first-year PhD student...
(Your existing text)

Research Interests
My research focuses on...
✅ Just filled in

Education
Ph.D. in Computer Science...
✅ Just filled in

Experience
Graduate Research Assistant...
✅ Just filled in

News & Updates
(Can be empty or add announcements)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```

**What's in this file:**
- Markdown text with `##` headings
- Your About Me text
- Research Interests ✅ Filled
- Education ✅ Filled
- Experience ✅ Filled
- News & Updates ⏳ Empty (optional)

---

### 3️⃣ `_data/navigation.yml` (Controls Top Menu)
**Location:** `/Users/wangzixian/zixianwang2022.github.io/_data/navigation.yml`

This file controls the **TOP NAVIGATION BAR**.

**What you see on the website:**
```
┌────────────────────────────────────┐
│ Publications | Blog Posts | CV      │
└────────────────────────────────────┘
```

**Current links:**
- Publications → `/publications/` (shows your research papers)
- Blog Posts → `/year-archive/` (your blog, currently empty)
- CV → `/cv/` (your curriculum vitae)

---

## Other Important Directories

### `_publications/` - Your Research Papers
**What shows:** Publications page at `/publications/`

Currently has 5 sample files. You'll replace these with your actual publications.

### `_posts/` - Your Blog Posts
**What shows:** Blog archive at `/year-archive/`

Currently empty (you deleted the samples). Add `.md` files here if you want blog posts.

### `images/` - Your Pictures & Files
**What shows:** Profile picture and other images

You'll add `profile.png` here (300×300px).

### `files/` - PDFs and Downloads
**What shows:** Downloadable resources

Place PDFs of your papers, CV, etc. here and link to them.

---

## The Complete Website Layout

```
┌─────────────────────────────────────────────────────────────────┐
│              https://zixianwang2022.github.io/                  │
├─────────────────────────────────────────────────────────────────┤
│  Publications  |  Blog Posts  |  CV                              │
│  ↑ From _data/navigation.yml                                     │
├──────────────────────┬──────────────────────────────────────────┤
│   LEFT SIDEBAR       │         MAIN CONTENT                     │
│ (from _config.yml)   │    (from _pages/about.md)                │
│                      │                                           │
│ [Photo]              │  # Welcome to My Academic Portfolio       │
│                      │                                           │
│ Zixian Wang          │  ## About Me                              │
│                      │  I am a first-year PhD student...        │
│ He/Him               │                                           │
│                      │  ## Research Interests                    │
│ First-year PhD       │  My research focuses on...               │
│ student at UIUC      │                                           │
│ advised by...        │  ## Education                             │
│                      │  Ph.D. in Computer Science...             │
│ 📧 Email             │                                           │
│ 🐙 GitHub            │  ## Experience                            │
│ 🔗 Scholar           │  Graduate Research Assistant...          │
│                      │                                           │
└──────────────────────┴──────────────────────────────────────────┘
```

---

## File Edit Workflow

When you edit `_config.yml`:
1. ✏️ Edit in VS Code
2. 💾 Save
3. 📤 Commit & push to GitHub
4. ⏳ Wait 30 seconds
5. 🌐 Visit website - sidebar shows your changes!

When you edit `_pages/about.md`:
1. ✏️ Edit in VS Code
2. 💾 Save
3. 📤 Commit & push to GitHub
4. ⏳ Wait 30 seconds
5. 🌐 Visit website - main content shows your changes!

---

## What's Currently Set Up ✅

- ✅ Site name: "Zixian Wang"
- ✅ Author name in sidebar: "Zixian Wang"
- ✅ Bio: "First-year PhD student at UIUC advised by Prof. Minjia Zhang"
- ✅ Pronouns: "He/Him"
- ✅ Email: "zixianw4@illinois.edu"
- ✅ GitHub: "zixianwang2022"
- ✅ About Me section: Written
- ✅ Research Interests: Filled in
- ✅ Education: Filled in
- ✅ Experience: Filled in
- ✅ Navigation: Clean (3 main pages)

## What Still Needs Work ⏳

- Profile picture: Add `images/profile.png`
- Academic profiles: Fill in Google Scholar, arXiv, ORCID if you have them
- News & Updates: Can stay empty or add updates
- Publications: Replace sample files with your actual papers
- CV: Update `/pages/cv.md` with your full CV

---

## Next Steps

1. **Add profile picture:**
   - Save your photo as 300×300 pixels
   - Name it `profile.png`
   - Place in `/images/` folder
   - Commit and push

2. **Add publications:**
   - Replace files in `_publications/` with your papers
   - Or delete sample files and leave empty for now

3. **Update CV:**
   - Edit `_pages/cv.md` with your full curriculum vitae

4. **Add optional social links:**
   - Fill in Google Scholar, arXiv, LinkedIn, etc. in `_config.yml`
   - Leave blank if you don't have them

---

## How to Check Your Changes

Visit: **https://zixianwang2022.github.io/**

After pushing changes, wait 30 seconds and refresh. You should see:
- Left sidebar with your name and bio
- Main content with About, Research Interests, Education, Experience
- Top menu with Publications, Blog Posts, CV

That's it! Your site is now live with your information! 🎉
