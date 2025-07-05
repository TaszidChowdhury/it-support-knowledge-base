# IT Helpdesk Knowledge Base 📚

A modern, beginner-friendly IT support knowledge base built with [MkDocs](https://www.mkdocs.org/) and the [Material theme](https://squidfunk.github.io/mkdocs-material/). Designed for self-service IT support, this knowledge base provides clear, step-by-step guides for common IT tasks.

![Knowledge Base Homepage](docs/assets/images/homepage.png)
*Modern, responsive homepage with easy navigation*

## 🚀 Features

- **📱 Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **🔍 Full-Text Search**: Find information quickly with the built-in search functionality
- **🎨 Modern UI**: Clean, professional Material Design theme
- **📖 Step-by-Step Guides**: Clear instructions for common IT tasks
- **🔗 Cross-References**: Easy navigation between related topics
- **⚡ Fast Loading**: Optimized for quick access to information

## 📋 Included Guides

| Guide | Description | Difficulty |
|-------|-------------|------------|
| [Setting Up a New Laptop](docs/setting-up-new-laptop.md) | Complete laptop setup from unboxing to productivity | Beginner |
| [Resetting Your Password](docs/resetting-password.md) | Password recovery for Windows and Google Workspace | Beginner |
| [Connecting to Wi-Fi](docs/connecting-to-wifi.md) | Wi-Fi setup for Windows and Mac | Beginner |
| [Installing Slack](docs/installing-slack.md) | Slack installation and setup | Beginner |
| [Installing Zoom](docs/installing-zoom.md) | Zoom installation and configuration | Beginner |
| [Setting Up Google Workspace](docs/setting-up-google-workspace.md) | Google Workspace account activation and setup | Beginner |
| [Configuring MFA](docs/configuring-mfa.md) | Multi-Factor Authentication setup | Intermediate |

![Guides Overview](docs/assets/images/guides-overview.png)
*Comprehensive list of available IT support guides*

## 🛠️ Technology Stack

- **MkDocs**: Static site generator
- **Material for MkDocs**: Modern, responsive theme
- **Markdown**: Easy-to-write and maintain content
- **Python**: Backend for local development
- **GitHub Pages**: Free hosting and deployment

## 📦 Installation & Setup

### Prerequisites

- Python 3.8 or higher
- Git (for version control)

### Local Development Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/TaszidChowdhury/it-support-knowledge-base.git
   cd it-support-knowledge-base
   ```

2. **Create a virtual environment:**
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Start the development server:**
   ```bash
   mkdocs serve
   ```

5. **Open your browser and visit:**
   ```
   http://127.0.0.1:8000/
   ```

![Local Development](docs/assets/images/local-development.png)
*Running the knowledge base locally for development*

### Production Deployment

#### Option 1: GitHub Pages (Recommended)

1. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Initial commit: IT Helpdesk Knowledge Base"
   git push origin main
   ```

2. **Enable GitHub Pages:**
   - Go to repository Settings → Pages
   - Set Source to "Deploy from a branch"
   - Select `main` branch and `/docs` folder
   - Save settings

3. **Your site will be available at:**
   ```
   https://taszidchowdhury.github.io/it-support-knowledge-base/
   ```

#### Option 2: Build Static Site

```bash
mkdocs build
```

This creates a `site/` directory with static HTML files that can be deployed to any web server.

![GitHub Pages Setup](docs/assets/images/github-pages-setup.png)
*GitHub Pages configuration for automatic deployment*

## 📁 Project Structure

```
it-support-knowledge-base/
├── docs/                          # Documentation files
│   ├── index.md                   # Homepage
│   ├── setting-up-new-laptop.md   # Laptop setup guide
│   ├── resetting-password.md      # Password reset guide
│   ├── connecting-to-wifi.md      # Wi-Fi connection guide
│   ├── installing-slack.md        # Slack installation guide
│   ├── installing-zoom.md         # Zoom installation guide
│   ├── setting-up-google-workspace.md  # Google Workspace setup
│   ├── configuring-mfa.md         # MFA configuration guide
│   └── assets/                    # Images and other assets
│       └── images/
├── mkdocs.yml                     # MkDocs configuration
├── requirements.txt               # Python dependencies
└── README.md                      # This file
```

## 🎨 Customization

### Adding New Guides

1. Create a new `.md` file in the `docs/` directory
2. Add the guide to the navigation in `mkdocs.yml`
3. Follow the existing format for consistency

### Customizing the Theme

Edit `mkdocs.yml` to customize colors, fonts, and other theme options:

```yaml
theme:
  name: material
  palette:
    - scheme: default
      primary: indigo
      accent: indigo
      toggle:
        icon: material/toggle-switch
        name: Switch to dark mode
    - scheme: slate
      primary: indigo
      accent: indigo
      toggle:
        icon: material/toggle-switch-off-outline
        name: Switch to light mode
```

### Adding Images

1. Place images in `docs/assets/images/`
2. Reference them in Markdown: `![Alt text](assets/images/filename.png)`

![Customization Example](docs/assets/images/customization.png)
*Example of theme customization options*

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch:** `git checkout -b feature/new-guide`
3. **Make your changes** and test locally
4. **Commit your changes:** `git commit -m "Add new guide: [Guide Name]"`
5. **Push to your fork:** `git push origin feature/new-guide`
6. **Create a Pull Request**

### Guide Writing Guidelines

- Use clear, step-by-step instructions
- Include screenshots for complex procedures
- Test all instructions before submitting
- Follow the existing format and style
- Use beginner-friendly language

## 📊 Usage Statistics

This knowledge base is designed to:
- **Reduce IT support tickets** by 40-60%
- **Improve user self-service** adoption
- **Speed up onboarding** for new employees
- **Standardize IT procedures** across the organization

![Usage Dashboard](docs/assets/images/usage-dashboard.png)
*Example usage statistics and impact metrics*

## 🔧 Troubleshooting

### Common Issues

**Port already in use:**
```bash
pkill -f mkdocs
mkdocs serve
```

**Theme not loading:**
```bash
pip install --upgrade mkdocs-material
```

**Build errors:**
```bash
mkdocs build --strict
```

### Getting Help

- Check the [MkDocs documentation](https://www.mkdocs.org/)
- Review [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) theme docs
- Open an issue on GitHub for bugs or feature requests

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [MkDocs](https://www.mkdocs.org/) for the excellent static site generator
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/) for the beautiful theme
- The open-source community for inspiration and tools

## 📞 Support

For questions or support:
- **Email:** it-support@company.com
- **Slack:** #it-helpdesk
- **GitHub Issues:** [Create an issue](https://github.com/TaszidChowdhury/it-support-knowledge-base/issues)

---

**Made with ❤️ for better IT support**

*Last updated: January 2025* 