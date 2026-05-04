# anothergrind.github.io
**Personal portfolio and academic website for Kamsi Ozorji**

![Academic Pages template example](images/homepage.png "anothergrind website")

## About

This is a personal portfolio website showcasing my academic work, projects, publications, talks, teaching experience, and blog. Built with Jekyll and hosted on GitHub Pages.

**Website:** https://anothergrind.github.io  
**About Me:** CS Student at University of Texas at Dallas | Incoming SWE Intern @ Atlassian

## Site Contents

- **Blog:** Thoughts and reflections on computer science and tech
- **Projects:** Showcase of personal and academic projects
- **CV:** Interactive CV and academic profile
- **Contact:** Ways to reach out and connect

## Quick Start

## Installation & Requirements

### System Dependencies

**Required:**
- Ruby 3.0 or higher
- Bundler
- Node.js
- Git

**Optional:** Docker and Docker Compose (for containerized development)

## Development Setup

### Option 1: Local Development

#### Prerequisites

**On Linux (Ubuntu/Debian):**
```bash
sudo apt update && sudo apt upgrade -y
sudo apt install build-essential gcc make ruby-dev ruby-bundler nodejs
```

**On macOS:**
```bash
brew install ruby node
gem install bundler
```

**On Windows:**
- Install [Ruby+Devkit](https://rubyinstaller.org/) (includes bundler)
- Install [Node.js](https://nodejs.org/)
- Install [Git for Windows](https://git-scm.com/download/win)

#### Setup Steps

1. Clone the repository:
```bash
git clone https://github.com/anothergrind/anothergrind.github.io.git
cd anothergrind.github.io
```

2. Install Ruby dependencies:
```bash
bundle install
```

If you encounter permission errors, install gems locally:
```bash
bundle config set --local path 'vendor/bundle'
bundle install
```

3. Start the development server:
```bash
bundle exec jekyll serve -l -H localhost
```

The site will be available at `http://localhost:4000` and will automatically rebuild on file changes.

### Option 2: Docker Development

Requires [Docker](https://www.docker.com/) and Docker Compose to be installed.

```bash
docker compose up
```

The site will be available at `http://localhost:4000`.

### Option 3: VS Code Dev Container

If using [Visual Studio Code](https://code.visualstudio.com/):

1. Install the [Dev Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
2. Press `F1` and run **Dev Containers: Reopen in Container**
3. VS Code will restart in the container and automatically build the site
4. Access it at `http://localhost:4000`

## Project Structure

```
├── _data/              # Site configuration data (authors, navigation)
├── _drafts/            # Unpublished blog posts
├── _includes/          # Reusable HTML components
├── _layouts/           # Page templates
├── _pages/             # Static pages (About, CV, Contact, etc.)
├── _portfolio/         # Portfolio project entries
├── _posts/             # Blog posts
├── _publications/      # Academic publications
├── _sass/              # Stylesheets
├── _talks/             # Talks and presentations
├── _teaching/          # Teaching experience entries
├── assets/             # Images, CSS, JS
├── files/              # Downloadable files (PDFs, etc.)
├── images/             # Site images
├── markdown_generator/ # Python tools for bulk content generation
├── _config.yml         # Jekyll configuration
└── Gemfile             # Ruby dependencies
```

## Content Management

### Adding Blog Posts

Create a new markdown file in `_posts/` with the filename format: `YYYY-MM-DD-title.md`

```markdown
---
title: "My Post Title"
date: 2026-05-04
categories: [blog]
tags: [tag1, tag2]
---

Your content here...
```

### Adding Publications

Create entries in `_publications/` following the existing format, or use the Python script in `markdown_generator/` to bulk-generate from a TSV file.

### Adding Portfolio Items

Add markdown or HTML files to `_portfolio/` directory with front matter metadata.

### Generating Content from TSV

Use the Jupyter notebooks in `markdown_generator/` to generate publication and talk entries in bulk from TSV files.

## Technologies Used

- **Jekyll** - Static site generator
- **Ruby** - Jekyll runtime
- **Minimal Mistakes Theme** - Base theme (customized)
- **GitHub Pages** - Hosting
- **Liquid** - Templating language
- **YAML** - Data format
- **Markdown** - Content format
- **SCSS** - Styling
- **Python** - Content generation tools
- **Docker** - Containerization

## License

This repository uses the MIT License. See [LICENSE](LICENSE) for details.

The website theme is based on [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) by Michael Rose.

## Attribution

This site is built using the [Academic Pages](https://academicpages.github.io/) template, which is based on the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) by Michael Rose (© 2016, released under MIT License).
