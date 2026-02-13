# Site Cleanup Guide

Your site has been cleaned up and is ready for your personal content! Here's what was done and what you need to do next.

## ✅ Changes Made

### 1. **Configuration Updates** (`_config.yml`)
   - Updated site URLs and repository references
   - Replaced all placeholder text with TODO comments for easy identification
   - Cleaned up author profile section with clear instructions
   - Organized social media and academic profile links with TODO markers

### 2. **Navigation Simplified** (`_data/navigation.yml`)
   - **Removed:** Talks, Teaching, Portfolio, Guide pages
   - **Kept:** Publications, Blog Posts, CV
   - Cleaner, more focused header menu

### 3. **Home Page Updated** (`_pages/about.md`)
   - Replaced template documentation with clean structure
   - Added sections ready for your content:
     - About Me
     - Research Interests
     - Education
     - Experience
     - News & Updates

### 4. **Sample Blog Posts Deleted**
   - All sample blog posts removed
   - `_posts/` directory is empty and ready for your content

## 🚀 What You Need to Do Next

### Step 1: Update Configuration (`_config.yml`)
Find all lines with `TODO:` and update them:
- **Your name** (appears in multiple places)
- **Site title and description**
- **Your email address**
- **GitHub username**
- **Add profile picture:** Save your image as `images/profile.png`
- **Academic profiles:** Add URLs to Google Scholar, ORCID, arXiv, etc. (leave blank if not applicable)
- **Social media:** Add your social profiles (leave blank if not applicable)

### Step 2: Complete Your About Page (`_pages/about.md`)
Replace the TODO comments with:
- Your name and introduction
- Research interests and expertise
- Educational background
- Professional experience
- Any news or updates you want to highlight

### Step 3: Add Your Publications (`_publications/`)
The directory already has 5 sample publication files. Each publication file should follow this format:

```markdown
---
title: "Your Paper Title"
collection: publications
permalink: /publication/2024-01-01-paper-title
excerpt: 'Brief description of the paper'
date: 2024-01-01
venue: 'Journal or Conference Name'
citation: 'Your Name, et al. (2024). "Your Paper Title." Journal/Conference Name.'
---

Optional abstract or additional information here.
```

**To generate publication files automatically:**
- Use the Jupyter notebooks in `markdown_generator/` directory
- Or manually create `.md` files in the `_publications/` format

### Step 4: Add Blog Posts (Optional) (`_posts/`)
To add blog posts, create files named: `YYYY-MM-DD-blog-post-title.md`

```markdown
---
title: 'Your Blog Post Title'
date: 2024-01-01
permalink: /posts/2024/01/blog-post/
tags:
  - tag1
  - tag2
---

Your blog content here.
```

### Step 5: Update Your CV (`_pages/cv.md`)
Edit the CV page to list your education, experience, and other accomplishments.

### Step 6: Add Your Profile Picture
1. Save your profile picture as `images/profile.png` (or update the filename in `_config.yml`)
2. Recommended size: 300x300 pixels

## 📋 Key Files to Customize

| File | Purpose |
|------|---------|
| `_config.yml` | Site configuration (name, bio, links) |
| `_pages/about.md` | Your home/about page |
| `_publications/` | Your research publications |
| `_pages/cv.md` | Your curriculum vitae |
| `_posts/` | Blog posts (currently empty) |
| `images/` | Profile picture and other images |

## 🔗 Useful Resources

- **Academic Pages Template:** https://github.com/academicpages/academicpages.github.io
- **Jekyll Documentation:** https://jekyllrb.com/docs/
- **GitHub Pages:** https://pages.github.com/

## 📝 Publication File Format Reference

Here's a template for creating publication files:

```markdown
---
title: "Paper Title Here"
collection: publications
permalink: /publication/YYYY-MM-DD-paper-slug
excerpt: 'Brief one-line summary'
date: YYYY-MM-DD
venue: 'Journal Name or Conference Name'
citation: 'Author1, Author2, et al. (YYYY). &quot;Paper Title.&quot; <i>Journal/Conference</i>.'
---

## Abstract
Your abstract here (optional).

## Recommended Citation
```

## 🎨 Customization Tips

1. **Change color theme:** Edit `site_theme` in `_config.yml` (options: default, air, sunrise, mint, dirt, contrast)
2. **Add more sections:** Duplicate page files in `_pages/` for competitions, projects, etc.
3. **Customize layout:** Edit files in `_layouts/` directory (for advanced users)

---

**Next Step:** Start by updating `_config.yml` with your information, then update `_pages/about.md` with your bio!
