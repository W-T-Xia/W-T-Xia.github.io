# W-T-Xia.github.io
This is 夏文韬(also known as 夏文韜 or Wen-Tao Xia)'s personal blog website.
Blogs are mainly written in Chinese(漢語).



# Personal Blog & Profile

> A multilingual, dark-mode-ready personal blog built with vanilla HTML, CSS, and JavaScript — powered by GitHub Pages.

---

## 📖 Version Log

### v1.4.0 — 2026-08-10
**Giscus Comments Integration**

- Added Giscus comment system for each blog post
- Comments are mapped via `pathname`, ensuring each article has its own independent comment thread
- Comment interface language follows the site's language selection (zhs/zht/eng)
- Comment theme automatically syncs with the site's dark/light mode toggle
- Comments are stored as GitHub Discussions in the repository, allowing admin review and management

---

### v1.3.0 — 2026-08-04
**Published Second Article: "愛在西元前"**

- Added new blog post `chen-jian.md` with full content
- Front matter (intro poem) and colophon (closing poem) formatted as italic + bold using inline HTML styles
- Added proper paragraph spacing between sections for better readability
- Removed second-person pronouns ("you/I") to reduce didactic tone

---

### v1.2.0 — 2026-08-02
**Dark / Light Theme Toggle**

- Added dark/light mode toggle with CSS variables
- Theme preference is saved in `localStorage` for persistence across sessions
- All UI elements adapt seamlessly to both themes
- Default theme is dark mode

---

### v1.1.0 — 2026-08-01
**Multilingual UI (zhs / zht / eng)**

- Complete UI internationalization with three language options: 简体中文 (ZHS:simplified Chinese), 繁體中文 (ZHT:traditional Chinese), English (英語)
- All interface text (navigation, buttons, profile, social labels) stored in `config/lang.json`
- Language selection is reflected in URL (`?lang=zhs|zht|eng`) and persists via browser history
- Social media labels (GitHub, Email) also support multilingual display
- Data externalization: personal profile moved to `config/profile.json`, social links extracted with `id`-based matching, article catalog moved to `posts/manifest.json` (single-language)

---

### v1.0.0 — 2026-07-30
**Initial Release — First Article: "Hello World"**

- Single-page architecture with **Personal Profile + Blog** layout
- Two-column responsive design (Profile sidebar + Main content area)
- Markdown rendering via `marked.js` library
- Blog post list with click-to-read functionality
- Published first article: "Hello World，我的第一篇博客"
- Basic CSS styling with glassmorphism effect
- Static data was initially hardcoded in JavaScript (externalized in later versions)

---

## 🚀 Technology Stack

| Component | Technology |
| :--- | :--- |
| Frontend | HTML5, CSS3, Vanilla JavaScript (ES6+) |
| Markdown Parsing | [marked.js](https://marked.js.org/) |
| Comments | [Giscus](https://giscus.app/) (powered by GitHub Discussions) |
| Hosting | [GitHub Pages](https://pages.github.com/) |
| Version Control | Git + GitHub |

---

## 📁 Project Structure
.
├── index.html # Main entry point (all logic included)
├── config/
│ ├── lang.json # UI translations (zhs/zht/eng)
│ └── profile.json # Personal info & social links
├── posts/
│ ├── manifest.json # Article catalog (single-language)
│ ├── hello-world.md # Blog post content
│ └── chen-jian.md # Blog post content
├── images/
│ └── avatar.jpg # Profile avatar
├── README.md # This file
├── .gitignore
└── LICENSE

text

---

## 🛠️ Quick Start

### Local Development
1. Clone the repository:
   ```bash
   git clone https://github.com/w-t-xia/w-t-xia.github.io.git
   cd w-t-xia.github.io
Open with VS Code and use Live Server extension, or run:

bash
npx serve .
Visit http://localhost:3000 to preview.

Deployment
Push to the main branch — GitHub Pages will automatically deploy the site at:

text
https://w-t-xia.github.io
🔧 Configuration
Add a New Blog Post
Create a Markdown file in posts/ (e.g., my-post.md)

Add an entry to posts/manifest.json:

json
{
    "id": "my-post",
    "date": "2026-08-10",
    "title": "My Post Title",
    "desc": "A short description for the archive page."
}
Push changes — the post will automatically appear in the article list.

Update Personal Info
Edit config/profile.json:

json
{
    "avatar": "images/avatar.jpg",
    "social": [
        { "id": "github", "url": "https://github.com/your-username" },
        { "id": "email", "url": "mailto:your-email@example.com" }
    ]
}
...and update corresponding translations in config/lang.json.

## 📝 License

**Code** (HTML/CSS/JS):  
Licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute the code for personal or commercial projects.

**Blog Content** (Markdown files in `posts/`):  
All rights reserved. Do not republish, reproduce, or commercialize without explicit written permission from the author.

---

## 👤 Author

**夏文韬(a.k.a.夏文韜 or Wen-Tao Xia)**  
Tongji University, Shanghai  
📧 w.t.xia.2005@gmail.com  

---

*Last updated: 2026-08-10*

---
