# Quick Edit Checklist: What to Fill In

This is your personal checklist of all the fields you need to update.

## 🎯 PRIORITY 1: Required for Your Site to Look Good

Update these in `_config.yml`:

### Left Sidebar Info
- [ ] `author.name` - Change from "Your Name" to **"Zixian Wang"**
- [ ] `author.bio` - Replace with your 1-2 sentence bio. Example: "PhD student at UIUC studying machine learning systems"
- [ ] `author.email` - ✅ Already has `zixianw4@illinois.edu` (looks good!)

### About Page
Update these in `_pages/about.md`:

- [ ] **Research Interests** section - Add 3-5 bullet points
- [ ] **Education** section - List your degrees
- [ ] **Experience** section - List your positions
- [ ] **News & Updates** section - Add any recent news (can be empty for now)

---

## 🎨 PRIORITY 2: Nice to Have (Profile Picture & Social Links)

### Profile Picture
- [ ] Add `profile.png` to `/images/` folder (300×300 px recommended)
  - This will appear at the top of your left sidebar

### Academic Profiles (Optional but Recommended)
Add your URLs if you have them:
- [ ] `author.googlescholar` - Your Google Scholar profile
- [ ] `author.arxiv` - Your arXiv author page
- [ ] `author.orcid` - Your ORCID ID
- [ ] `author.github` - ✅ Already has "zixianwang2022" (good!)

### Social Media (Optional)
- [ ] `author.linkedin` - Your LinkedIn profile URL
- [ ] `author.twitter` - Your Twitter/X handle
- [ ] `author.website` - Your personal website (if you have one)

---

## 📝 Current Status

### ✅ Already Done
- Name: "Zixian Wang" is set
- Email: "zixianw4@illinois.edu" is set
- GitHub: "zixianwang2022" is set
- Location: "University of Illinois Urbana Champaign" is set
- Pronouns: "He/Him" is set

### ⏳ Still Needs Work
- Author name in sidebar: Still says "Your Name"
- Bio: Still says "Your short bio here"
- Profile picture: Not added yet
- Research Interests: Empty
- Education: Empty
- Experience: Empty

---

## 📋 Exact Changes to Make

### Step 1: Update Left Sidebar (in `_config.yml`)

**Find this section:**
```yaml
author:
  name             : "Your Name"              # ← Change this
  bio              : "Your short bio here"    # ← Change this
```

**Change to something like:**
```yaml
author:
  name             : "Zixian Wang"
  bio              : "First-year PhD student studying ML systems at UIUC"
```

### Step 2: Fill Your About Page (in `_pages/about.md`)

**For Research Interests, change from:**
```markdown
## Research Interests
<!-- TODO: List your research interests and areas of focus -->
```

**To something like:**
```markdown
## Research Interests
- Machine learning systems and optimization
- Distributed computing and systems
- Performance analysis and profiling
```

**For Education, change from:**
```markdown
## Education
<!-- TODO: Add your educational background -->
```

**To something like:**
```markdown
## Education
**Ph.D. in Computer Science** (In Progress, 2023-Present)  
University of Illinois Urbana-Champaign, Advisor: Prof. Minjia Zhang

**B.S. in Computer Science**  
[Your Undergraduate University], [Year]
```

**For Experience, change from:**
```markdown
## Experience
<!-- TODO: Add your professional experience -->
```

**To something like:**
```markdown
## Experience
**Graduate Research Assistant** (Aug 2023 - Present)  
University of Illinois Urbana-Champaign  
Advisor: Prof. Minjia Zhang

**[Previous Position]** ([Dates])  
[Company/University]  
[Brief description]
```

---

## How to Tell Your Changes Work

1. **Edit a file** (e.g., change "Your Name" to "Zixian Wang")
2. **Save the file** in VS Code
3. **Commit & push** to GitHub
4. **Wait 30 seconds** (GitHub rebuilds your site)
5. **Visit** https://zixianwang2022.github.io/
6. **Your changes appear!** ✨

You should see:
- Left sidebar shows "Zixian Wang" (not "Your Name")
- Left sidebar shows your bio
- Main content shows your research interests, education, etc.

---

## Example of What Your Page Will Look Like

After you fill everything in:

```
┌────────────────────────┐
│  [YOUR PHOTO]          │
│                        │
│  Zixian Wang           │ ← Changed from "Your Name"
│  ────────────────────  │
│                        │
│  First-year PhD        │ ← Changed from placeholder
│  student studying ML   │
│  systems at UIUC       │
│                        │
│  📧 zixianw4@illinois  │
│  🐙 zixianwang2022     │
│  🔗 Google Scholar     │
│                        │
└────────────────────────┘

    Welcome to My Academic Portfolio

    About Me
    I am a first-year PhD student at University of 
    Illinois Urbana Champaign (UIUC) advised by 
    Prof. Minjia Zhang.

    Research Interests
    - Machine learning systems and optimization
    - Distributed computing and systems
    - Performance analysis and profiling

    Education
    Ph.D. in Computer Science (In Progress, 2023-Present)
    University of Illinois Urbana-Champaign

    Experience
    Graduate Research Assistant (Aug 2023 - Present)
    University of Illinois Urbana-Champaign
    ...
```

---

## Troubleshooting

**Q: I changed something but it's not showing up on my website**
A: Wait 30 seconds after pushing to GitHub. GitHub Pages takes a moment to rebuild.

**Q: How do I see what's on my site?**
A: Visit https://zixianwang2022.github.io/ after committing changes.

**Q: Can I preview changes locally?**
A: Yes, but requires installing Jekyll (optional). We can set that up if you want instant feedback while editing.

**Q: Which file controls what I see on the home page?**
A: `_pages/about.md` (the main content) and `_config.yml` (the left sidebar)

---

**Ready to edit? Start with updating `author.name` and `author.bio` in `_config.yml`!** 🚀
