# Banghao Chi's Academic Website

This repository contains the source code for [Banghao Chi's](https://biboyqg.github.io) academic website, built with Jekyll and hosted on GitHub Pages. The site showcases research publications, projects, and academic work in ML Systems.

## 🌐 Live Site

Visit the website at: [biboyqg.github.io](https://biboyqg.github.io)

## 📋 About

This is a Jekyll-based static site designed specifically for academic researchers and engineers. The site features:

- **Research Publications**: Organized display of academic papers with abstracts, PDFs, and code links
- **Project Showcase**: Visual portfolio of research projects and implementations
- **Responsive Design**: Modern, clean interface optimized for both desktop and mobile
- **Performance Optimized**: Automatic thumbnail generation for fast loading
- **SEO Friendly**: Proper meta tags, sitemaps, and structured data

## 🏗️ Technical Stack

- **Static Site Generator**: Jekyll
- **Hosting**: GitHub Pages
- **Styling**: Sass/SCSS
- **Domain**: Custom domain with CNAME configuration
- **Image Optimization**: Automatic thumbnail generation

## 📁 Project Structure

```
├── _data/              # YAML data files for content management
│   ├── work_experience.yml  # Work experience and positions
│   └── awards.yml           # Awards and honors
├── _layouts/           # Jekyll layout templates
├── _posts/            # Research publications and blog posts
├── _sass/             # Sass stylesheets and components
├── images/            # Full-size images and figures
├── tn/images/         # Auto-generated thumbnails
├── pdfs/              # Research papers and documents
├── _config.yml        # Jekyll configuration
├── style.scss         # Main stylesheet
└── _make_thumbnails.sh # Thumbnail generation script
```

## 🚀 Getting Started

### Prerequisites

- Ruby (2.7 or higher)
- Jekyll
- Git

### Local Development

1. **Clone the repository**

   ```bash
   git clone https://github.com/biboyqg/biboyqg.github.io.git
   cd biboyqg.github.io
   ```

2. **Install dependencies**

   ```bash
   gem install jekyll bundler
   bundle install
   ```

3. **Generate thumbnails** (if you've added new images)

   ```bash
   chmod +x _make_thumbnails.sh
   ./_make_thumbnails.sh
   ```

4. **Run the development server**

   ```bash
   bundle exec jekyll serve
   ```

5. **View the site**
   Open your browser to `http://localhost:4000`

### Adding New Content

#### Adding a Research Publication

Create a new file in `_posts/` with the format `YYYY-MM-DD-title.markdown`:

```yaml
---
layout: post
title: "Your Paper Title"
date: 2025-01-01 22:21:59 +00:00
image: /images/your_image.png
categories: [CATEGORY]
author: "Your Name"
authors: "<strong>Your Name</strong>, Co-author Name, et. al."
venue: "Conference/Journal Name"
paper: /pdfs/your_paper.pdf
code: https://github.com/your-username/your-repo
---
Brief description or abstract of your paper...
```

#### Adding Work Experience

Add entries to `_data/work_experience.yml`:

**For Academic/Research Positions:**
```yaml
- title: "Research Intern"
  organization: "Organization Name"
  organization_short: "SHORT"  # Optional abbreviation
  organization_url: "https://org.edu/"  # Optional
  location: "City/University"
  period: "Fall 2024 - Spring 2025"
```

**For Course-Related Positions:**
```yaml
- title: "Teaching Assistant"
  course_code: "CS 357"
  course_url: "https://course-website.edu/"  # Optional
  location: "University"
  period: "Fall 2024 - Spring 2025"
```

#### Adding Awards & Honors

Add entries to `_data/awards.yml`:

```yaml
- year: "2025"
  award: "Award Name (description)"
  institution: "Institution Name"
```

#### Adding Images

1. Add full-size images to the `images/` directory
2. Run the thumbnail generation script: `./_make_thumbnails.sh`
3. Thumbnails will be automatically created in `tn/images/`

## ⚙️ Configuration

Key configuration options in `_config.yml`:

- **Personal Information**: Update name, email, social links
- **Site URL**: Configure for your domain
- **Navigation**: Customize header and footer links
- **Analytics**: Add Google Analytics tracking (optional)

## 🎨 Customization

### Styling

- Main styles: `style.scss`
- Component styles: `_sass/` directory
- Color scheme and typography can be customized in the Sass variables

### Layout Templates

- `_layouts/default.html`: Main page template
- `_layouts/post.html`: Individual post template

### Categories

The site supports multiple post categories:

- Research publications
- Projects
- Blog posts
- Conference presentations

## 🔧 Technical Features

### Data-Driven Content Management

The site uses Jekyll's `_data` directory for managing structured content:

- **Work Experience**: Automatically renders different formats for academic positions ("Research Intern at NCSA") vs. courses ("Teaching Assistant for CS 357")
- **Awards & Honors**: Table format with year, award, and institution columns
- **Easy Updates**: Modify YAML files instead of editing HTML templates

### Automatic Thumbnail Generation

The `_make_thumbnails.sh` script automatically generates optimized thumbnails for all images, improving page load times while maintaining visual quality.

### SEO Optimization

- Automatic sitemap generation
- Open Graph meta tags
- Structured data for academic publications
- Custom permalinks for clean URLs

### Performance

- Sass compilation and compression
- Image optimization through thumbnails
- Minimal JavaScript for fast loading
- Mobile-responsive design

## 📝 Content Guidelines

### Research Publications
- **Images**: Use high-quality images for research figures and project screenshots
- **PDFs**: Store papers and documents in the `pdfs/` directory
- **Code Links**: Include GitHub repositories for reproducible research
- **Abstracts**: Keep post descriptions concise but informative

### Work Experience & Awards
- **Consistency**: Use consistent date formats (e.g., "Fall 2024 - Spring 2025")
- **URLs**: Include relevant links to organizations, courses, or institutions when available
- **Abbreviations**: Use `organization_short` for commonly abbreviated organizations (e.g., "NCSA", "SSAIL")
- **Course Codes**: Use standard course numbering (e.g., "CS 357", "CS 409")

## 🤝 Contributing

This template is open for use by other researchers. Feel free to:

1. Fork this repository
2. Customize for your own academic website
3. Submit improvements via pull requests

**Please respect copyright**: Do not reuse personal content from `images/`, `pdfs/`, or `_posts/` directories.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Built on [Jekyll Now](https://github.com/barryclark/jekyll-now)
- Design inspired by [Jon Barron's website](https://jonbarron.info/)
- Hosted on GitHub Pages

## 📧 Contact

**Banghao Chi**

- Email: banghao2@illinois.edu
- GitHub: [@biboyqg](https://github.com/biboyqg)
- LinkedIn: [banghao-chi](https://linkedin.com/in/banghao-chi-550737276)

---

_This website serves as a portfolio for academic research and professional work in ML Systems._
