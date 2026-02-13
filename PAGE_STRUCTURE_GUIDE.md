# How Your About Page Maps to the Website

## Visual Structure of Your Page

Here's exactly what appears where on your website when you visit `/`:

```
┌─────────────────────────────────────────────────────────────────┐
│                         YOUR WEBSITE                             │
├──────────────────────────────┬──────────────────────────────────┤
│    LEFT SIDEBAR              │      MAIN CONTENT AREA            │
│  (from _config.yml)          │   (from _pages/about.md)          │
│                              │                                    │
│  Profile Picture             │  # Welcome to My Academic Port... │
│  avatar (profile.png)        │                                    │
│                              │  ## About Me                       │
│  Your Sidebar Name           │  I am a first-year PhD student... │
│  (author.name)               │                                    │
│                              │  ## Research Interests            │
│  Short bio                   │  [Your research interests]        │
│  (author.bio)                │                                    │
│                              │  ## Education                     │
│  Social Links                │  [Your education]                 │
│  (all your URLs)             │                                    │
│                              │  ## Experience                    │
│                              │  [Your experience]                │
│                              │                                    │
│                              │  ## News & Updates                │
│                              │  [Any announcements]              │
│                              │                                    │
└──────────────────────────────┴──────────────────────────────────┘
```

## Your Current about.md File Breakdown

Here's what each part of your markdown file does:

### Front Matter (Between `---` lines at the top)
```markdown
---
permalink: /              # This makes it appear at www.yoursite.com/
title: "About"           # Page title (shown in browser tab)
author_profile: true     # IMPORTANT: Shows the left sidebar with your info!
redirect_from: 
  - /about/
  - /about.html          # Old URLs that redirect here
---
```
**What it does:** Sets up the page properties and displays your sidebar.

### Main Content (Below the `---`)

```markdown
# Welcome to My Academic Portfolio
```
**What it does:** Large heading at the top of your page. Users see this first.

```markdown
## About Me
I am a first-year PhD student at University of Illinois Urbana Champaign (UIUC) advised my Prof. Minjia Zhang.
```
**What it does:** Creates a section with a smaller heading, followed by your text. This is visible to visitors!

```markdown
## Research Interests
<!-- TODO: Add your research interests and areas of focus -->
```
**What it does:** Creates another section. The comment (`<!-- -->`) is invisible to visitors—only you see it in the editor.

```markdown
## Education
<!-- TODO: Add your educational background -->
```
**What it does:** Another section ready for your education details.

## How Markdown Formatting Works

| Markdown | Appears As | Example |
|----------|-----------|---------|
| `# Heading` | Large heading | # Your Title |
| `## Subheading` | Medium heading | ## About Me |
| `### Sub-subheading` | Smaller heading | ### PhD Details |
| `**bold text**` | **bold text** | **Bold** |
| `*italic text*` | *italic text* | *Italic* |
| `[link text](url)` | clickable link | [Google](https://google.com) |
| `- bullet point` | • bullet point | - First point |
| `1. numbered` | 1. numbered | 1. First |
| `<!-- comment -->` | invisible | Not shown to visitors |

## What You See on Your Published Page

When someone visits your site, they see:

```
┌──────────────────────────────────────────────────┐
│ Welcome to My Academic Portfolio                 │
│                                                   │
│ About Me                                          │
│ I am a first-year PhD student at University of   │
│ Illinois Urbana Champaign (UIUC) advised my      │
│ Prof. Minjia Zhang.                              │
│                                                   │
│ Research Interests                                │
│ [You add content here]                            │
│                                                   │
│ Education                                         │
│ [You add content here]                            │
│                                                   │
│ Experience                                        │
│ [You add content here]                            │
│                                                   │
│ News & Updates                                    │
│ [You add content here]                            │
└──────────────────────────────────────────────────┘
(with LEFT SIDEBAR showing your profile pic, name, bio, social links)
```

## Where Your _config.yml Shows Up

The file `_config.yml` controls the **LEFT SIDEBAR** content:

```yaml
author:
  avatar: "profile.png"              → Your profile picture (top of sidebar)
  name: "Your Name"                  → Your name (under picture)
  bio: "Your short bio here"         → Short biography text
  email: "your.email@example.com"    → Shows as clickable email link
  github: "zixianwang2022"           → Shows as GitHub profile link
  linkedin: # URL                    → Shows as LinkedIn link (if filled)
  googlescholar: # URL               → Shows as Google Scholar link (if filled)
  [other profiles...]                → All appear as clickable icons
```

## Quick Editing Examples

### Example 1: Add Your Research Interests
**Currently:**
```markdown
## Research Interests
<!-- TODO: List your research interests and areas of focus -->
```

**Change to:**
```markdown
## Research Interests
My research focuses on:
- Machine learning systems
- Distributed computing
- Performance optimization
```

**Result on page:**
```
Research Interests
My research focuses on:
• Machine learning systems
• Distributed computing
• Performance optimization
```

### Example 2: Add Education
**Currently:**
```markdown
## Education
<!-- TODO: Add your educational background -->
```

**Change to:**
```markdown
## Education
**Ph.D. in Computer Science** (Current)  
University of Illinois Urbana-Champaign, 2023-Present

**B.S. in Computer Science**  
Shanghai Jiao Tong University, 2019-2023
```

**Result on page:**
```
Education
Ph.D. in Computer Science (Current)
University of Illinois Urbana-Champaign, 2023-Present

B.S. in Computer Science
Shanghai Jiao Tong University, 2019-2023
```

### Example 3: Add Experience
**Currently:**
```markdown
## Experience
<!-- TODO: Add your professional experience -->
```

**Change to:**
```markdown
## Experience
**Research Assistant** at UIUC (2023-Present)  
Working on distributed machine learning systems under Prof. Minjia Zhang.

**Intern** at Tech Company (Summer 2022)  
Optimized performance of data processing pipelines.
```

## The Flow: Editing → Publishing → Viewing

1. **You edit** `_pages/about.md` → Save
2. **GitHub** automatically rebuilds your site (takes ~30 seconds)
3. **Your changes appear** at https://zixianwang2022.github.io/

No special preview needed—just edit, commit, and refresh the webpage after a few seconds!

## Navigation Toolbar

Remember, your navigation bar (at the very top) is controlled by `_data/navigation.yml`:

```yaml
main:
  - title: "Publications"     → Links to /publications/
    url: /publications/
  
  - title: "Blog Posts"       → Links to /year-archive/
    url: /year-archive/
  
  - title: "CV"               → Links to /cv/
    url: /cv/
```

These are separate pages that you can also customize!

---

## Summary

- **Left sidebar** = configured in `_config.yml` (author section)
- **Main content** = your markdown in `_pages/about.md`
- **Top navigation** = configured in `_data/navigation.yml`
- **Markdown syntax** = turns into formatted text and headings
- **Workflow**: Edit file → Commit to GitHub → Refresh your browser (30 sec later)

Start editing `_pages/about.md` and you'll see your changes live on GitHub pages!
