# 🎨 Modern Portfolio Template

A beautiful, customizable portfolio template that anyone can use! No coding required - just run the setup wizard, add your content, and deploy.

**Perfect for:** Developers, designers, freelancers, students, or anyone wanting a professional online presence.

🚀 **[View Demo](https://tian102.github.io/tianpretorius.github.io/)** | 📖 **[Documentation](docs/TEMPLATE_SETUP.md)** | 🐛 **[Report Issue](https://github.com/tian102/tianpretorius.github.io/issues)**

---

## ✨ Why This Template?

- ⚡ **5-Minute Setup** - Interactive wizard guides you through configuration
- 🎨 **Fully Customizable** - Colors, fonts, content - all via simple config file
- 📝 **Markdown Content** - Write blog posts and projects in markdown
- 🚀 **One-Click Deploy** - Deploy to GitHub Pages with a single command
- 📱 **Responsive Design** - Looks great on all devices
- 🎯 **No Frameworks** - Pure HTML/CSS/JS for fast loading
- ♿ **Accessible** - Built with accessibility in mind
- 📊 **Feature Toggles** - Enable/disable sections as needed

---

## 🚀 Quick Start

### Option 1: Interactive Setup (Recommended)

```bash
# 1. Use this template (click "Use this template" button on GitHub)
# OR clone the repository
git clone https://github.com/tian102/tianpretorius.github.io.git my-portfolio
cd my-portfolio

# 2. Install dependencies
npm install

# 3. Run the setup wizard
npm run setup
# Answer the questions - it takes 2 minutes!

# 4. Build your site
npm run build

# 5. Preview locally
npx live-server
```

### Option 2: Manual Configuration

```bash
# 1. Clone and install
git clone https://github.com/tian102/tianpretorius.github.io.git my-portfolio
cd my-portfolio
npm install

# 2. Edit config/template.config.js with your information

# 3. Build and preview
npm run build
npx live-server
```

### Option 3: GitHub Template

1. Click **"Use this template"** button on GitHub
2. Name your repository `yourusername.github.io`
3. Clone your new repository
4. Follow steps 2-5 from Option 1

📖 **Full setup guide:** [docs/TEMPLATE_SETUP.md](docs/TEMPLATE_SETUP.md)

---

## 🎨 Features

### 🏠 Homepage
- Animated hero section with role typing animation
- Interactive "flip card" hero image (click to reveal)
- Customizable gradient effects
- Social media links

### 👤 About
- Multi-section about page
- Skills showcase
- Timeline/experience section
- Resume download link

### � Projects
- Project showcase with thumbnails
- Markdown-based project details
- Technology tags
- Live demo and GitHub links
- Filtering and search
- Featured projects section

### 📝 Blog
- Full-featured blog system
- Markdown-based posts
- Tags and categories
- Search functionality
- Table of contents auto-generation
- Reading time estimates
- Featured posts

### 📧 Contact
- Contact form integration
- Social media links
- Email link
- Optional contact page

### ⚙️ Configuration
- **One config file** - Everything in `config/template.config.js`
- **Setup wizard** - Interactive CLI configuration
- **Theme system** - Custom colors and fonts
- **Feature toggles** - Enable/disable sections
- **Content management** - Centralized in `data/site-content.json`

### 🛠️ Developer Features
- **Build system** - Compiles markdown to JSON
- **Validation** - Ensures config is correct
- **Clean script** - Remove example content
- **Live preview** - Test before deploying
- **No dependencies** - Vanilla JS, no frameworks

---

## 📁 Project Structure

```
modern-portfolio-template/
├── config/
│   └── template.config.js     # 👈 YOUR CONFIGURATION HERE
├── content/
│   ├── blog/posts/            # 👈 YOUR BLOG POSTS (markdown)
│   └── projects/posts/        # 👈 YOUR PROJECTS (markdown)
├── data/
│   ├── site-content.json      # Generated site content
│   ├── blog-posts.json        # Generated from markdown
│   └── projects.json          # Generated from markdown
├── scripts/
│   ├── setup-wizard.js        # Interactive setup
│   ├── build-content.js       # Markdown compiler
│   ├── apply-theme.js         # Theme generator
│   ├── validate-config.js     # Config validation
│   └── clean-example-content.js # Remove examples
├── docs/                      # 📖 Documentation
│   ├── TEMPLATE_SETUP.md      # Setup guide
│   ├── CUSTOMIZATION.md       # Customization guide
│   ├── DEPLOYMENT.md          # Deployment guide
│   ├── TROUBLESHOOTING.md     # Common issues
│   └── CONTRIBUTING.md        # Contribution guide
├── css/
│   ├── style.css              # Main styles
│   ├── blog.css               # Blog/project styles
│   └── theme-variables.css    # Generated theme (auto)
├── js/
│   ├── main.js                # Navigation & common
│   ├── content-loader.js      # Content management
│   ├── config-handler.js      # Feature toggles
│   ├── blog.js                # Blog functionality
│   ├── projects.js            # Projects functionality
│   └── index.js               # Homepage features
├── assets/                    # Your images & files
├── *.html                     # Page templates
└── package.json               # Scripts & metadata
```

---

## 📝 Adding Content

### Blog Posts

```bash
# Create new post directory
mkdir content/blog/posts/my-first-post
cd content/blog/posts/my-first-post

# Create post file
New-Item index.md
```

```markdown
---
title: "My First Blog Post"
date: "2024-01-15"
tags: ["tutorial", "web development"]
featured: true
---

# My First Post

Your content here in markdown...

## Subheading

More content...
```

```bash
# Build and preview
npm run build
npx live-server
```

### Projects

```bash
# Create project directory
mkdir content/projects/posts/my-project
cd content/projects/posts/my-project

# Create project file
New-Item index.md
```

```markdown
---
title: "My Awesome Project"
description: "Short description"
technologies: ["React", "Node.js", "MongoDB"]
github: "https://github.com/username/project"
demo: "https://demo.com"
thumbnail: "assets/thumbnail.jpg"
featured: true
---

# Project Details

Detailed description...
```

📖 **Full content guide:** [docs/TEMPLATE_SETUP.md#adding-content](docs/TEMPLATE_SETUP.md#adding-content)

---

## 🎨 Customization

### Change Colors

```javascript
// config/template.config.js
theme: {
    primaryColor: '#3498db',  // Your brand color
    accentColor: '#e74c3c'    // Accent color
}
```

```bash
npm run build:theme  # Apply theme
```

### Toggle Features

```javascript
// config/template.config.js
features: {
    blog: true,       // Show/hide blog
    projects: true,   // Show/hide projects
    contact: true     // Show/hide contact
}
```

### Change Fonts

```javascript
// config/template.config.js
theme: {
    fontFamily: 'Poppins, sans-serif',
    codeFontFamily: 'Fira Code, monospace'
}
```

📖 **Full customization guide:** [docs/CUSTOMIZATION.md](docs/CUSTOMIZATION.md)

---

## 🚀 Deployment

### Deploy to GitHub Pages

```bash
# 1. Ensure repository is named: yourusername.github.io

# 2. Build your site
npm run build

# 3. Commit and push
git add .
git commit -m "Deploy portfolio"
git push origin main

# 4. Enable GitHub Pages
# Settings → Pages → Source: main branch → Save

# 5. Your site is live at: https://yourusername.github.io
```

### Other Platforms

- **Netlify:** Connect GitHub repo, auto-deploys on push
- **Vercel:** Import GitHub repo, instant deployment
- **Cloudflare Pages:** Fast CDN, free tier

📖 **Full deployment guide:** [docs/DEPLOYMENT.md](docs/DEPLOYMENT.md)

---

## 📋 Available Commands

| Command | Description |
|---------|-------------|
| `npm run setup` | Run interactive setup wizard |
| `npm run build` | Build everything (validate + content + theme) |
| `npm run build:content` | Compile markdown to JSON |
| `npm run build:theme` | Generate theme CSS from config |
| `npm run validate` | Validate configuration |
| `npm run clean` | Remove example content |
| `npx live-server` | Preview site locally |

---

## 🆘 Troubleshooting

**Issue:** Config validation fails
```bash
npm run validate  # See specific errors
```

**Issue:** Content not showing
```bash
npm run build:content  # Rebuild content
# Check data/*.json files
```

**Issue:** Theme not applied
```bash
npm run build:theme  # Regenerate theme CSS
# Hard refresh browser (Ctrl+Shift+R)
```

**Issue:** Build errors
```bash
npm install  # Reinstall dependencies
npm run build  # Try again
```

📖 **Full troubleshooting guide:** [docs/TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md)

---

## 📚 Documentation

- 📖 [Setup Guide](docs/TEMPLATE_SETUP.md) - Complete setup walkthrough
- 🎨 [Customization Guide](docs/CUSTOMIZATION.md) - Customize everything
- 🚀 [Deployment Guide](docs/DEPLOYMENT.md) - Deploy to hosting platforms
- 🔧 [Troubleshooting Guide](docs/TROUBLESHOOTING.md) - Common issues & solutions
- 🤝 [Contributing Guide](docs/CONTRIBUTING.md) - Help improve this template

---

## 🌟 Examples

Want to see what others have built? Check out these portfolios using this template:

- [Example 1](#) - Software Engineer
- [Example 2](#) - UX Designer
- [Example 3](#) - Freelance Developer

*(Add your portfolio here by opening a PR!)*

---

## 🤝 Contributing

Contributions are welcome! Please read the [Contributing Guide](docs/CONTRIBUTING.md) first.

### Ways to Contribute
- 🐛 Report bugs
- 💡 Suggest features
- 📝 Improve documentation
- 🔧 Submit pull requests
- ⭐ Star this repository

---

## � License

MIT License - feel free to use this template for personal or commercial projects!

---

## 🙏 Acknowledgments

- Built with vanilla HTML, CSS, and JavaScript
- Markdown parsing with [marked.js](https://marked.js.org/)
- Icons from [Font Awesome](https://fontawesome.com/) (if used)
- Inspired by modern portfolio designs

---

## 📞 Support

- 📖 [Documentation](docs/TEMPLATE_SETUP.md)
- 💬 [Discussions](https://github.com/tian102/tianpretorius.github.io/discussions)
- 🐛 [Report Issue](https://github.com/tian102/tianpretorius.github.io/issues)

---

## ⭐ Show Your Support

If this template helped you, give it a ⭐ star on GitHub!

---

**Made with ❤️ for the developer community**

*Turn this template into your dream portfolio in under 10 minutes!*