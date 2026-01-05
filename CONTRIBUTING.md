# Contributing to Just-Newbies

Thank you for your interest in contributing to Just-Newbies! 
We welcome contributions from everyone, and you don't need to be a coding expert to make a difference. 
If you've mastered a topic to the point where you can explain it in simple words -so clearly that even a 5-year-old child could understand it,
then we need you!

## **Writing Content Contributions**

This is a community-to-community work, and we highly value human-written explanations. 
Your unique perspective, experience, and way of explaining concepts are what make this project special.
You can contribute to existing chapters or articles by improving explanations, adding examples, or suggesting better ways to present information. 
You're also encouraged to suggest entirely new topics that you think would benefit newcomers in the field. 
Whether it's simplifying technical jargon, creating relatable analogies, or restructuring content for better clarity.

Your name will always reside in the articles you've helped create or improve,
ensuring you receive proper recognition for your contributions to the community.
We value every contributor and believe in giving credit where credit is due.

**Important:** We strongly discourage the use of AI for writing academic content. We want authentic, 
human-written explanations that come from your genuine understanding and teaching experience. 
This personal touch is what resonates with learners and creates real educational value.

#### **Where to find the content files?**

Just-Newbies uses the Hugo framework, where you write and modify your content only in `.md` files.  
You can modify or create new files inside the [`content/english`](https://github.com/Just-OSG/Just-Newbies/tree/main/content/english) folder for the English version and the [`content/arabic`](https://github.com/Just-OSG/Just-Newbies/tree/main/content/arabic) folder for arabic written content.  
If you don't know what an `.md` (Markdown) file is, please check out this [article](https://www.markdownguide.org/basic-syntax/) to learn the basic syntax.

If you have an idea for a new topic that would help newbies? 
Open an issue with the "topic suggestion" label and describe what you'd like to see covered. 
Include why you think this topic is important and how it would benefit learners.


## **Technical Contributions**

Technical contributions include bug fixes, feature implementations, website improvements, and infrastructure enhancements.
Before you start working on any issue, you must comment under the issue you want to work on to state that you are taking it.
This helps confirm that your contribution is valid, prevents duplicated work, and keeps the workflow clear and organized.

### **Prerequisites**

Before you start contributing to the project, make sure you have the following installed:

- **Git**: For version control and cloning the repository
- **Hugo Extended**: Version 0.112.0 or higher (the extended version is required for SCSS/SASS processing)
- **A text editor**: VS Code, Sublime Text, or any editor of your choice

### **What is Hugo?**

Hugo is a fast and flexible static site generator written in Go. Unlike traditional content management systems (CMS), Hugo generates static HTML files from your content (written in Markdown) and templates. This makes the website incredibly fast, secure, and easy to deploy. Hugo uses a simple folder structure where you write content in Markdown files, and it automatically generates the corresponding HTML pages.

### **Setting Up the Project Locally**

Follow these steps to get the project running on your local machine:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Just-OSG/Just-Newbies.git
   cd Just-Newbies
   ```

2. **Install [Hugo Extended](https://gohugo.io/installation/)**:
   - **Windows**: Use `winget install Hugo.Hugo.Extended` (winget is pre-installed on Windows 10/11)
   - **macOS**: Use Homebrew: `brew install hugo`
   - **Linux**: Use your package manager or download from [Hugo Releases](https://github.com/gohugoio/hugo/releases)

3. **Verify Hugo installation**:
   ```bash
   hugo version
   ```
   Make sure it says "extended" in the output.

4. **Run the development server**:
   ```bash
   hugo server
   ```
Since the project supports multiple languages, you can access:
   - **English version**: `http://localhost:1313/`
   - **Arabic version**: `http://localhost:1314/`
   
   Hugo will automatically reload the page when you make changes to the content or theme files.

5. **Run with drafts** (if you want to preview draft content):
   ```bash
   hugo server -D
   ```

### **Project Structure**

Understanding the project structure will help you navigate and contribute effectively:

```
Just-Newbies/
├── config.yaml              # Main configuration file (site settings, menus, languages)
├── content/                 # All content files (Markdown)
│   ├── arabic/              # Arabic content
│   │   ├── _index.md        # Arabic homepage content
│   │   ├── about.md         # About page in Arabic
│   │   └── get-to-know-the-terms/  # Chapter/section folders
│   └── english/             # English content
│       ├── _index.md        # English homepage content
│       ├── about.md         # About page in English
│       └── get-to-know-the-terms/  # Chapter/section folders
├── themes/                  # Hugo themes
│   └── just-newbies/        # Custom theme for the project
│       ├── layouts/         # HTML templates
│       ├── assets/          # SCSS, JS, and other assets
│       └── static/          # Static files (images, fonts)
├── static/                  # Static files accessible from root
│   └── img/                 # Images used in content
├── public/                  # Auto Generated site (don't touch this)
├── resources/               # Hugo's cache (auto-generated)
└── scripts/                 # Utility scripts for development
```

**Key folders to know**:

- **`content/`**: This is where you'll spend most of your time. Add or edit `.md` files here to create or modify content.
- **`themes/just-newbies/`**: Contains the theme files. Edit layouts, styles (SCSS), and scripts here for design changes.
- **`config.yaml`**: Configuration file for site-wide settings, navigation menus, language settings, and theme parameters.
- **`static/`**: Place images, fonts, or any static assets that need to be served as-is.
- **`public/`**: Auto-generated folder containing the built website. Never edit files here directly.

### **Making Changes**

- **Content changes**: Edit or create `.md` files in the `content/` folder
- **Style changes**: Edit SCSS files in `themes/just-newbies/assets/`
- **Layout changes**: Edit HTML templates in `themes/just-newbies/layouts/`
- **Configuration**: Edit `config.yaml` for site-wide settings

After making changes, Hugo's development server will automatically refresh your browser to show the updates.

---

If you have any questions about contributing, feel free to open an issue or [reach out](mailto:justosgroup@gmail.com) to the maintainers.
