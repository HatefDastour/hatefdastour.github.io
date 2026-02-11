# Dr. Hatef Dastour - Personal Academic Website

[![Website](https://img.shields.io/badge/Website-hatefdastour.github.io-blue)](https://hatefdastour.github.io/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Jekyll](https://img.shields.io/badge/Built%20with-Jekyll-red.svg)](https://jekyllrb.com/)

Welcome to the repository for my personal academic website, hosted at [hatefdastour.github.io](https://hatefdastour.github.io/). This site showcases my research, publications, teaching, and professional activities.

## 👤 About

**Dr. Hatef Dastour**  
- **Position:** Assistant Teaching Professor of Data Science and Analytics, AI Faculty Fellow
- **Institution:** University of Missouri, Columbia
- **Research Focus:** Geospatial AI, Environmental Science, Machine Learning, Remote Sensing
- **Education:** Dual PhDs in Geomatics Engineering and Mathematics & Statistics from the University of Calgary

## 🌐 Website Overview

This website serves as a comprehensive portfolio of my academic and professional work:

- **Research:** Publications, ongoing projects, and research interests
- **Teaching:** Course materials, syllabi, and educational resources
- **Publications:** Peer-reviewed articles, conference papers, and technical reports
- **Talks:** Conference presentations and invited seminars
- **Notes:** Technical blog posts and tutorials
- **CV:** Comprehensive academic curriculum vitae

## 🛠️ Technical Details

### Built With

- **Static Site Generator:** [Jekyll](https://jekyllrb.com/) 3.x
- **Theme:** Modified Academic Pages theme
- **Hosting:** GitHub Pages
- **Markup:** Markdown with Kramdown
- **Styling:** Sass/SCSS
- **JavaScript:** Minimal, progressive enhancement

### Repository Structure

```
hatefdastour.github.io/
├── _config.yml              # Site configuration
├── _config.dev.yml          # Development configuration
├── _data/                   # Data files (navigation, etc.)
├── _includes/               # HTML includes and components
├── _layouts/                # Page layouts
├── _pages/                  # Main site pages
├── _publications/           # Publication entries
├── _research/               # Research project entries
├── _teaching/               # Teaching materials
├── _talks/                  # Talk and presentation entries
├── _notes/                  # Blog posts and notes
├── _sass/                   # Stylesheets
├── assets/                  # CSS, JS, and other assets
├── images/                  # Image files
├── files/                   # PDFs and other documents
├── markdown_generator/      # Scripts for generating markdown
├── Gemfile                  # Ruby dependencies
└── README.md               # This file
```

## 🚀 Local Development

### Prerequisites

- Ruby 2.5 or higher
- Bundler gem
- Git

### Setup Instructions

1. **Clone the repository:**

```bash
git clone https://github.com/HatefDastour/hatefdastour.github.io.git
cd hatefdastour.github.io
```

2. **Install dependencies:**

```bash
bundle install
```

3. **Serve the site locally:**

```bash
# Production configuration
bundle exec jekyll serve

# Development configuration (with future posts and drafts)
bundle exec jekyll serve --config _config.yml,_config.dev.yml
```

4. **View the site:**

Open your browser to `http://localhost:4000`

### Making Changes

The site will automatically rebuild when you modify files. Refresh your browser to see changes.

**Note:** Changes to `_config.yml` require restarting the Jekyll server.

## 📝 Content Management

### Adding Publications

Create a new markdown file in `_publications/` with the following front matter:

```yaml
---
title: "Your Paper Title"
collection: publications
permalink: /publication/paper-slug
excerpt: 'Brief description of the paper'
date: YYYY-MM-DD
venue: 'Journal or Conference Name'
paperurl: 'https://doi.org/...'
citation: 'Your citation format'
---
```

### Adding Teaching Materials

Create a new markdown file in `_teaching/` following the existing template structure.

### Adding Research Projects

Create a new markdown file in `_research/` with relevant project information.

### Adding Talks

Create a new markdown file in `_talks/` with presentation details and slides (if available).

### Adding Blog Posts

Create a new markdown file in `_notes/` for technical notes, tutorials, or blog posts.

## 🎨 Customization

### Modifying Site Configuration

Edit `_config.yml` to update:
- Site title and description
- Author information
- Social media links
- Google Analytics tracking (if enabled)
- SEO settings

### Updating Navigation

Modify `_data/navigation.yml` to change menu items.

### Styling

Custom styles are in `_sass/` and can be modified to change the site's appearance.

## 📊 Content Collections

The site uses Jekyll collections for organizing content:

- **publications:** Academic papers and articles
- **research:** Research projects and initiatives
- **teaching:** Course materials and syllabi
- **talks:** Conference presentations and seminars
- **notes:** Technical blog posts and tutorials

Each collection has its own directory and can be browsed on the live site.

## 🔧 Markdown Generator

The `markdown_generator/` directory contains Python scripts for batch-generating markdown files from CSV or TSV data. Useful for importing:
- Multiple publications from BibTeX or CSV
- Course listings
- Talk schedules

## 📄 License

This website repository is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Content (publications, research descriptions, teaching materials) © Hatef Dastour. All rights reserved unless otherwise noted.

## 🤝 Acknowledgments

This website is built upon the excellent [Academic Pages](https://github.com/academicpages/academicpages.github.io) template, which is a fork of the [Minimal Mistakes Jekyll theme](https://mmistakes.github.io/minimal-mistakes/).

## 📧 Contact

For questions about this website or collaboration inquiries:

- **Website:** [hatefdastour.github.io](https://hatefdastour.github.io/)
- **Email:** dastourh@missouri.edu
- **GitHub:** [@HatefDastour](https://github.com/HatefDastour)
- **LinkedIn:** [hatefdastour](https://linkedin.com/in/hatefdastour)
- **Google Scholar:** [Profile](https://scholar.google.ca/citations?user=ZWWezMsAAAAJ&hl=en)
- **ORCID:** [0000-0002-2119-9077](https://orcid.org/0000-0002-2119-9077)

## 🔗 Quick Links

- [🏠 Home](https://hatefdastour.github.io/)
- [📚 Publications](https://hatefdastour.github.io/publications/)
- [🔬 Research](https://hatefdastour.github.io/research/)
- [👨‍🏫 Teaching](https://hatefdastour.github.io/teaching/)
- [🎤 Talks](https://hatefdastour.github.io/talks/)
- [📝 Notes](https://hatefdastour.github.io/notes/)
- [📄 CV](https://hatefdastour.github.io/cv/)

---

**Last Updated:** February 2026  
**Repository:** [github.com/HatefDastour/hatefdastour.github.io](https://github.com/HatefDastour/hatefdastour.github.io)