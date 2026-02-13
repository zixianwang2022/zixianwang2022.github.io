# 🌐 Your Website Visual Guide

## Exactly What Visitors See

Here's a visual representation of your website at **https://zixianwang2022.github.io/**

```
╔════════════════════════════════════════════════════════════════════════════╗
║                     Zixian Wang - Academic Portfolio                       ║
║ ─────────────────────────────────────────────────────────────────────────── ║
║  [Publications] [Blog Posts] [CV]                                           ║
╠══════════════════════════════════════════════════════════════════════════════╣
║                                                                              ║
║  ┌─────────────────────────┐   ┌──────────────────────────────────────────┐ ║
║  │                         │   │ Welcome to My Academic Portfolio          │ ║
║  │    [PHOTO SPACE]        │   │                                          │ ║
║  │   (once you add         │   │ About Me                                  │ ║
║  │    profile.png)         │   │ ──────────────────────────────────────── │ ║
║  │                         │   │ I am a first-year PhD student at UIUC    │ ║
║  │ Zixian Wang             │   │ advised by Prof. Minjia Zhang.            │ ║
║  │ He/Him                  │   │                                          │ ║
║  │                         │   │ Research Interests                        │ ║
║  │ First-year PhD          │   │ ──────────────────────────────────────── │ ║
║  │ student at UIUC         │   │ My research focuses on:                  │ ║
║  │ advised by Prof.        │   │ - Machine learning systems               │ ║
║  │ Minjia Zhang            │   │ - Distributed computing                  │ ║
║  │                         │   │ - Performance optimization                │ ║
║  │ ─────────────────────── │   │                                          │ ║
║  │                         │   │ Education                                 │ ║
║  │ 📧 zixianw4@illinois... │   │ ──────────────────────────────────────── │ ║
║  │                         │   │ Ph.D. in Computer Science (In Progress)   │ ║
║  │ 🐙 zixianwang2022       │   │ University of Illinois Urbana-Champaign  │ ║
║  │ (GitHub profile link)   │   │ 2023-Present                              │ ║
║  │                         │   │ Advisor: Prof. Minjia Zhang               │ ║
║  │ [Other profiles will    │   │                                          │ ║
║  │  appear as you add      │   │ Experience                                │ ║
║  │  them in _config.yml]   │   │ ──────────────────────────────────────── │ ║
║  │                         │   │ Graduate Research Assistant              │ ║
║  └─────────────────────────┘   │ University of Illinois Urbana-Champaign  │ ║
║                                 │ Aug 2023-Present                          │ ║
║                                 │ Working on machine learning systems      │ ║
║                                 │ research under Prof. Minjia Zhang.       │ ║
║                                 │                                          │ ║
║                                 │ News & Updates                            │ ║
║                                 │ ──────────────────────────────────────── │ ║
║                                 │ (Add any announcements here)              │ ║
║                                 │                                          │ ║
║                                 └──────────────────────────────────────────┘ ║
║                                                                              ║
╚══════════════════════════════════════════════════════════════════════════════╝
```

## What's Currently Showing

### ✅ Left Sidebar (Configured in _config.yml)
- Profile picture placeholder (add your photo)
- **Name:** Zixian Wang
- **Pronouns:** He/Him  
- **Bio:** First-year PhD student at UIUC advised by Prof. Minjia Zhang
- **Email:** zixianw4@illinois.edu (clickable link)
- **GitHub:** zixianwang2022 (clickable link)

### ✅ Main Content (From _pages/about.md)
- **Welcome header**
- **About Me section** - Your introduction
- **Research Interests** - Machine learning, distributed computing, performance
- **Education** - PhD at UIUC
- **Experience** - Research Assistant role
- **News & Updates** - Currently empty (optional)

### ✅ Top Navigation (From _data/navigation.yml)
- **Publications** link
- **Blog Posts** link  
- **CV** link

---

## What Happens When Visitors Click Navigation Links

### Publications Page
```
/publications/ → Shows all research papers from _publications/ folder
Currently has: 5 sample publication files (you'll replace these)
```

### Blog Posts Page
```
/year-archive/ → Shows all blog posts from _posts/ folder
Currently: Empty (you deleted the samples)
Can add posts here if you want to blog
```

### CV Page
```
/cv/ → Shows your curriculum vitae
Edit: _pages/cv.md
```

---

## Text Formatting Examples

Everything in your `about.md` supports Markdown formatting:

| You write... | It appears as... |
|--------------|-----------------|
| `**bold text**` | **bold text** |
| `*italic text*` | *italic text* |
| `# Heading` | Large heading |
| `## Subheading` | Medium heading |
| `- bullet point` | • bullet point |
| `1. numbered` | 1. numbered item |
| `[Link text](url)` | [Link text](url) |

### Example: Better formatted Research Interests
You could write:
```markdown
## Research Interests
I'm passionate about building efficient machine learning systems. My research interests include:

- **Machine Learning Systems:** Optimization and scalability of ML training
- **Distributed Computing:** Fault tolerance and performance in distributed systems  
- **Performance Analysis:** Profiling and identifying bottlenecks in complex systems
```

It would display as:
```
Research Interests
I'm passionate about building efficient machine learning systems. 
My research interests include:

• Machine Learning Systems: Optimization and scalability of ML training
• Distributed Computing: Fault tolerance and performance in distributed systems
• Performance Analysis: Profiling and identifying bottlenecks in complex systems
```

---

## How to Make Your Page Even Better

### Add a Profile Picture
1. Find a professional headshot (300×300 pixels)
2. Save as `profile.png` in `/images/` folder
3. Commit & push → appears in sidebar!

### Add Academic Profiles
In `_config.yml`, add your URLs:
```yaml
author:
  googlescholar: "https://scholar.google.com/citations?user=YOUR_ID"
  arxiv: "https://arxiv.org/a/yourname"
  orcid: "https://orcid.org/YOUR-ID"
  linkedin: "https://linkedin.com/in/yourname"
```

### Add Publications
Replace files in `_publications/` with your papers

### Update Your Full CV
Edit `_pages/cv.md` with complete CV information

### Add News/Updates
Fill in the "News & Updates" section with recent announcements:
```markdown
## News & Updates
- **Feb 2024:** Paper accepted to OSDI!
- **Jan 2024:** Started PhD at UIUC
- **Dec 2023:** Graduated from SJTU
```

---

## The Publishing Workflow

```
┌─────────────────────────────┐
│ 1. Edit a file in VS Code   │
│    (e.g., _pages/about.md)  │
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│ 2. Save the file            │
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│ 3. Commit & push to GitHub  │
│    (git push)               │
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│ 4. GitHub detects changes   │
│    Rebuilds your site       │
│    (takes ~30 seconds)      │
└────────────┬────────────────┘
             ↓
┌─────────────────────────────┐
│ 5. Visit your website       │
│    https://zixianwang...    │
│    Changes are LIVE! ✨     │
└─────────────────────────────┘
```

---

## Your Site vs Template

| Feature | Your Site | Status |
|---------|-----------|--------|
| Home page | ✅ Clean about page | Ready! |
| Publications | Template structure | Ready for your papers |
| Blog | Empty (optional) | Ready if you want |
| CV | Template structure | Ready to fill |
| Sidebar | Your info | Done! |
| Navigation | 3 pages (clean) | Done! |
| Talks | ❌ Removed | Not needed |
| Teaching | ❌ Removed | Not needed |
| Portfolio | ❌ Removed | Not needed |

---

## Next Actionable Steps

1. **Commit your current changes** (if not done)
2. **Add profile picture** (Optional but recommended)
3. **Wait 30 seconds**, then visit your site
4. **See your name and bio appear in the sidebar!** 🎉

---

**Your site is LIVE! Every edit you make appears within minutes!**
