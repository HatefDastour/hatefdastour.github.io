# Dr. Hatef Dastour - Personal Academic Website

[![Website](https://img.shields.io/badge/Website-hatefdastour.github.io-blue?style=flat-square&logo=github)](https://hatefdastour.github.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![Jekyll](https://img.shields.io/badge/Built%20with-Jekyll-red.svg?style=flat-square&logo=jekyll)](https://jekyllrb.com/)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-222222?style=flat-square&logo=github)](https://pages.github.com/)
[![Last Commit](https://img.shields.io/github/last-commit/HatefDastour/hatefdastour.github.io?style=flat-square)](https://github.com/HatefDastour/hatefdastour.github.io/commits/master)

> 🌐 **Live Site:** [hatefdastour.github.io](https://hatefdastour.github.io/)

Welcome to the repository for my personal academic website. This site showcases my research in Geospatial AI and Environmental Science, teaching materials, publications, and professional activities.

---

## 👤 About Dr. Hatef Dastour

**Current Position:**  
Assistant Teaching Professor of Data Science and Analytics | AI Faculty Fellow  
University of Missouri, Columbia

**Academic Background:**
- **PhD in Geomatics Engineering** - University of Calgary
- **PhD in Mathematics & Statistics** - University of Calgary

**Research Expertise:**
- 🛰️ Geospatial AI and Remote Sensing
- 🌍 Environmental Science and Climate Modeling
- 🤖 Machine Learning and Deep Learning
- 🔥 Forest Fire Prediction and Risk Assessment
- 💧 Flood Modeling and Sustainability
- 🧠 Natural Language Processing and Large Language Models

**Academic Impact:**
- 25+ peer-reviewed publications
- Graduate-level instruction in NLP, LLMs, and Cloud Computing
- Industry experience as a Data Scientist
- Developing computational frameworks for environmental challenges

---

## 🌐 Website Sections

This website serves as a comprehensive portfolio of my academic and professional work:

| Section | Description | Link |
|---------|-------------|------|
| 🏠 **Home** | Introduction and overview | [Visit](https://hatefdastour.github.io/) |
| 📚 **Publications** | Peer-reviewed articles and conference papers | [View Publications](https://hatefdastour.github.io/publications/) |
| 🔬 **Research** | Current and past research projects | [Explore Research](https://hatefdastour.github.io/research/) |
| 👨‍🏫 **Teaching** | Course materials and syllabi | [Teaching Portfolio](https://hatefdastour.github.io/teaching/) |
| 🎤 **Talks** | Conference presentations and seminars | [View Talks](https://hatefdastour.github.io/talks/) |
| 📝 **Notes** | Technical blog posts and tutorials | [Read Notes](https://hatefdastour.github.io/notes/) |
| 📄 **CV** | Comprehensive curriculum vitae | [Download CV](https://hatefdastour.github.io/cv/) |

---

## 🛠️ Technical Stack

### Core Technologies

- **Static Site Generator:** [Jekyll](https://jekyllrb.com/) 3.x
- **Theme:** Modified [Academic Pages](https://github.com/academicpages/academicpages.github.io) (fork of Minimal Mistakes)
- **Hosting:** [GitHub Pages](https://pages.github.com/)
- **Markup:** Markdown with [Kramdown](https://kramdown.gettalong.org/)
- **Styling:** Sass/SCSS
- **Icons:** Font Awesome
- **Analytics:** Google Analytics (optional)

### Key Features

✅ Responsive design optimized for all devices  
✅ SEO-friendly structure  
✅ Fast loading times  
✅ Accessible and standards-compliant  
✅ Easy content management through Markdown  
✅ Automatic site generation from collections  
✅ Academic-focused layout and components

---

## 📁 Repository Structure

```plaintext
hatefdastour.github.io/
├── 📄 _config.yml              # Main site configuration
├── 📄 _config.dev.yml          # Development-specific settings
├── 📁 _data/                   # Data files (navigation, UI text)
│   └── navigation.yml          # Site menu structure
├── 📁 _includes/               # Reusable HTML components
│   ├── header.html
│   ├── footer.html
│   └── ...
├── 📁 _layouts/                # Page templates
│   ├── default.html
│   ├── single.html
│   └── ...
├── 📁 _pages/                  # Main site pages
│   ├── about.md
│   ├── cv.md
│   └── ...
├── 📁 _publications/           # Publication entries (Markdown)
├── 📁 _research/               # Research project descriptions
├── 📁 _teaching/               # Course materials and syllabi
├── 📁 _talks/                  # Talk and presentation entries
├── 📁 _notes/                  # Blog posts and technical notes
├── 📁 _sass/                   # Stylesheets (SCSS)
├── 📁 assets/                  # Compiled CSS, JS, fonts
├── 📁 images/                  # Image files and profile photos
├── 📁 files/                   # PDFs, documents, datasets
├── 📁 markdown_generator/      # Python scripts for batch content
├── 📁 talkmap/                 # Geographic visualization of talks
├── 📄 Gemfile                  # Ruby dependencies
├── 📄 LICENSE                  # MIT License
└── 📄 README.md               # This file
```

---

## 🚀 Local Development

### Prerequisites

Before you begin, ensure you have the following installed:

- **Ruby** 2.5 or higher ([Installation Guide](https://www.ruby-lang.org/en/documentation/installation/))
- **Bundler** gem: `gem install bundler`
- **Git** ([Download Git](https://git-scm.com/downloads))

### Setup Instructions

#### 1. Clone the Repository

```bash
git clone https://github.com/HatefDastour/hatefdastour.github.io.git
cd hatefdastour.github.io
```

#### 2. Install Ruby Dependencies

```bash
bundle install
```

This installs Jekyll and all required gems specified in the `Gemfile`.

#### 3. Serve the Site Locally

**Production mode:**
```bash
bundle exec jekyll serve
```

**Development mode** (includes drafts and future posts):
```bash
bundle exec jekyll serve --config _config.yml,_config.dev.yml
```

**With live reload:**
```bash
bundle exec jekyll serve --livereload
```

#### 4. View the Site

Open your browser and navigate to:
```
http://localhost:4000
```

The site will automatically rebuild when you modify files (except `_config.yml`, which requires a server restart).

### Troubleshooting

**Port already in use:**
```bash
bundle exec jekyll serve --port 4001
```

**Clear cache and rebuild:**
```bash
bundle exec jekyll clean
bundle exec jekyll serve
```

---

## 📝 Content Management Guide

### Adding Publications

Create a new file in `_publications/` with the naming convention: `YYYY-MM-DD-title.md`

```yaml
---
title: "Your Paper Title"
collection: publications
permalink: /publication/paper-slug
excerpt: 'Brief description of the paper (1-2 sentences)'
date: 2025-01-15
venue: 'Journal Name or Conference'
paperurl: 'https://doi.org/10.xxxx/xxxxx'
citation: 'Author(s). (Year). Title. <i>Venue</i>. Volume(Issue), pages.'
---

Optional extended description or abstract goes here.
```

### Adding Research Projects

Create a file in `_research/` with project details:

```yaml
---
title: "Research Project Title"
permalink: /research/project-slug
excerpt: "Brief project summary"
date: 2025-01-01
tags:
  - machine-learning
  - geospatial-ai
---

Detailed project description, methodology, findings, and links to publications or code.
```

### Adding Teaching Materials

Create a file in `_teaching/` for each course:

```yaml
---
title: "Course Number: Course Title"
collection: teaching
type: "Graduate/Undergraduate course"
permalink: /teaching/course-slug
venue: "University of Missouri, Department Name"
date: 2025-01-15
location: "Columbia, Missouri"
---

Course description, objectives, topics covered, and links to materials.
```

### Adding Talks and Presentations

Create a file in `_talks/`:

```yaml
---
title: "Presentation Title"
collection: talks
type: "Conference/Invited Talk/Seminar"
permalink: /talks/talk-slug
venue: "Conference or Event Name"
date: 2025-03-15
location: "City, State/Country"
---

Talk abstract and description. Include links to slides or video recordings.
```

### Adding Blog Posts (Notes)

Create a file in `_notes/`:

```yaml
---
title: 'Tutorial: Topic Name'
date: 2025-02-10
permalink: /notes/tutorial-slug
tags:
  - python
  - machine-learning
  - tutorial
---

Your blog post content in Markdown format.
```

---

## 🎨 Customization

### Site Configuration

Edit `_config.yml` to customize:

```yaml
# Site Settings
title: "Dr. Hatef Dastour"
description: "Academic website for Dr. Hatef Dastour"
url: "https://hatefdastour.github.io"

# Author Information
author:
  name: "Hatef Dastour"
  bio: "Assistant Teaching Professor | AI Faculty Fellow"
  location: "Columbia, Missouri"
  email: "dastourh@missouri.edu"
  
# Social Links
social:
  - title: "github"
    url: "https://github.com/HatefDastour"
  - title: "linkedin"
    url: "https://linkedin.com/in/hatefdastour"
```

### Navigation Menu

Modify `_data/navigation.yml`:

```yaml
- title: "Publications"
  url: /publications/
  
- title: "Research"
  url: /research/
  
- title: "Teaching"
  url: /teaching/
```

### Styling and Theme

Custom styles are located in `_sass/`. Key files:

- `_variables.scss` - Colors, fonts, spacing
- `_page.scss` - Page layouts
- `_masthead.scss` - Header/navigation
- `_footer.scss` - Footer styling

---

## 🔧 Advanced Features

### Markdown Generator Scripts

The `markdown_generator/` directory contains Python scripts for batch-generating content:

**Generate publications from CSV:**
```bash
cd markdown_generator
python publications.py
```

**Generate talks from CSV:**
```bash
python talks.py
```

These scripts are useful when importing multiple items from spreadsheets or BibTeX files.

### Talk Map Visualization

Generate an interactive map of your talks:

```bash
python talkmap.py
```

Or use the Jupyter notebook:
```bash
jupyter notebook talkmap.ipynb
```

### SEO and Analytics

The site includes:
- Automatic sitemap generation
- Meta tags for social media sharing
- Google Scholar meta tags for publications
- Optional Google Analytics integration

---

## 📊 Jekyll Collections

The site uses Jekyll collections to organize different content types:

| Collection | Directory | Purpose |
|------------|-----------|----------|
| `publications` | `_publications/` | Academic papers and articles |
| `research` | `_research/` | Research projects and initiatives |
| `teaching` | `_teaching/` | Course materials and syllabi |
| `talks` | `_talks/` | Presentations and seminars |
| `notes` | `_notes/` | Blog posts and tutorials |

Each collection is automatically:
- Listed on its respective archive page
- Indexed for search engines
- Rendered with appropriate templates
- Organized chronologically

---

## 🔒 Privacy and Analytics

This website respects user privacy:
- No tracking cookies by default
- Optional Google Analytics can be enabled in `_config.yml`
- No third-party advertising
- Open-source and transparent code

---

## 📄 License

**Code:** This repository's code is licensed under the **MIT License** - see [LICENSE](LICENSE) for details.

**Content:** Academic content (publications, research descriptions, teaching materials, images) © 2026 Hatef Dastour. All rights reserved unless otherwise noted.

**Attribution:** Built upon the [Academic Pages](https://github.com/academicpages/academicpages.github.io) template, which is a fork of [Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/) by Michael Rose.

---

## 🤝 Contributing

Found a bug or have a suggestion? Please:
1. Open an issue describing the problem or enhancement
2. Fork the repository
3. Create a feature branch
4. Submit a pull request

---

## 🙏 Acknowledgments

This website builds upon excellent open-source projects:

- **[Academic Pages](https://github.com/academicpages/academicpages.github.io)** - Template designed for academics
- **[Minimal Mistakes](https://mmistakes.github.io/minimal-mistakes/)** - Flexible Jekyll theme by Michael Rose
- **[Jekyll](https://jekyllrb.com/)** - Static site generator
- **[GitHub Pages](https://pages.github.com/)** - Free hosting for academic websites
- **Font Awesome** - Icon library

---

## 📧 Contact Information

**Dr. Hatef Dastour**  
Assistant Teaching Professor of Data Science and Analytics  
AI Faculty Fellow  
University of Missouri, Columbia

### Connect With Me

- 🌐 **Website:** [hatefdastour.github.io](https://hatefdastour.github.io/)
- 📧 **Email:** [dastourh@missouri.edu](mailto:dastourh@missouri.edu)
- 💼 **LinkedIn:** [linkedin.com/in/hatefdastour](https://linkedin.com/in/hatefdastour)
- 🐙 **GitHub:** [@HatefDastour](https://github.com/HatefDastour)
- 🎓 **Google Scholar:** [Profile](https://scholar.google.ca/citations?user=ZWWezMsAAAAJ&hl=en)
- 🔬 **ORCID:** [0000-0002-2119-9077](https://orcid.org/0000-0002-2119-9077)
- 🐦 **ResearchGate:** [Profile](https://www.researchgate.net/profile/Hatef-Dastour)

### Office & Collaboration

For research collaborations, speaking engagements, or academic inquiries, please reach out via email.

---

## 📅 Site Status

**Last Updated:** February 2026  
**Status:** ✅ Active and Maintained  
**Content Updates:** Regular additions of publications, teaching materials, and blog posts

---

## 📈 Repository Stats

![GitHub repo size](https://img.shields.io/github/repo-size/HatefDastour/hatefdastour.github.io?style=flat-square)
![GitHub language count](https://img.shields.io/github/languages/count/HatefDastour/hatefdastour.github.io?style=flat-square)
![GitHub top language](https://img.shields.io/github/languages/top/HatefDastour/hatefdastour.github.io?style=flat-square)

---

<div align="center">

**[⬆ Back to Top](#dr-hatef-dastour---personal-academic-website)**

 Made with ❤️ using Jekyll and GitHub Pages

</div>