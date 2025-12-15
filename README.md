Understood — you want a **complete, final, full `README.md`** that contains **everything**, fully cleaned, formatted, styled, and ready to paste directly into GitHub.

Below is the **entire README.md**, with **no omissions**.

If you want, I can also export it as a downloadable `.md` file afterward.

---

# **FINAL COMPLETE README.md**

````markdown
<h1 align="center">Peace Development Fund – UN Modelling Project</h1>

<p align="center">
  <b>Website Repository</b>
</p>

<p align="center">
  <a href="https://jekyllrb.com/">
    <img src="https://img.shields.io/badge/built%20with-Jekyll-red.svg" alt="Built with Jekyll">
  </a>
  <a href="https://www.zerostatic.io/docs/jekyll-advance/">
    <img src="https://img.shields.io/badge/theme-Jekyll%20Advance%20Pro-blue.svg" alt="Jekyll Advance Pro">
  </a>
  <a href="https://desa-eapd.github.io/modelling-project/">
    <img src="https://img.shields.io/badge/website-live%20site-green.svg" alt="Live Site">
  </a>
  <img src="https://img.shields.io/badge/status-active-success.svg" alt="Status: active">
</p>

---

This repository hosts the source code for the **Peace and Development Fund (PDF) – UN Modelling Project** website.

The official website is available at:  
👉 **https://desa-eapd.github.io/modelling-project/**

The site is built with **Jekyll** using the **Jekyll Advance Pro Theme**, and is designed to present:

- project information  
- country and thematic updates  
- modelling results and policy simulations  
- newsletters and knowledge products  

in a structured and accessible way for policymakers, partners, and stakeholders.

---

# 1. Project Overview

## Project Title  
**Rebuilding better and greener from the COVID-19 pandemic through enhanced design and implementation of sustainable national recovery strategies based on policy simulations**

## Objective  
Strengthen the capacity of government agencies to better utilize data and analytical tools to inform national development strategies through quantitative modelling.

## Duration  
**2023–2027**

## Target Countries  
*TBD*

## Main Activities  
- Identify planning and data gaps where modelling can enhance decision-making  
- Assess and customise modelling approaches (macro, micro-simulation, CLEWS)  
- Conduct workshops and modelling capacity development  
- Provide technical and advisory support to national governments  
- Produce policy documents informed by simulation results  
- Support participation in UN-level dialogues (ECOSOC, HLPF, etc.)  
- Publish modelling outputs, newsletters, and reports  

---

# 2. Theme: Jekyll Advance Pro

**Jekyll Advance Pro** is a premium multi-purpose theme designed for structured content, clean design, and scalable websites.

- **Live Demo:** https://jekyll-advance.netlify.app/  
- **Documentation:** https://www.zerostatic.io/docs/jekyll-advance/

![Theme Screenshot](https://www.zerostatic.io/theme/jekyll-advance/jekyll-advance-screenshot.png)

The project uses the theme to:

- Manage blog posts through **collections** (`_posts`)  
- Generate category-based navigation  
- Implement structured pages for project documentation  
- Publish newsletters and modelling updates  
- Render HTML through templates in `_layouts`  

---

# 3. Repository Structure

```text
.
├── collections/
│   ├── _posts/          # Blog/news posts and updates
│   ├── news/            # Newsletters and periodic publications
│   └── …                # Additional collections as required
│
├── pages/               # Static pages (about, countries, project, home, services)
│
├── categories/          # Category landing pages for filtering
│
├── assets/
│   └── images/
│        └── gen/
│             ├── blog/    
│             ├── content/ 
│             └── home/    
│
├── _layouts/            # Liquid/HTML templates
│
├── _config.yml          # Jekyll configuration
└── README.md
````

---

## 3.1 Posts (`collections/_posts`)

Used for:

* Project updates
* Modelling articles
* Country activities
* Training summaries

**Naming format:**

```
YYYY-MM-DD-title.md
```

**Example front matter:**

```yaml
---
layout: post
title: "National CLEWS Training – Philippines"
category: philippines
image: /assets/images/gen/blog/philippines-training.png
---
```

---

## 3.2 Pages (`pages/`)

For static project information pages.

**Example:**

```yaml
---
layout: project
title: "About the Modelling Project"
permalink: /about/
---
```

---

## 3.3 Categories (`categories/`)

Each category page is a filtering template.

**Example:**

```yaml
---
layout: category
title: "Philippines"
category: philippines
---
```

---

## 3.4 Newsletters (`collections/news`)

Store newsletters as:

* PDF
* Markdown `.md`

Naming examples:

```
2025-q1-newsletter.pdf
2024-midyear-update.md
```

---

## 3.5 Images (`assets/images/gen`)

Subfolders:

* `blog/` – images used in posts
* `content/` – illustrations inside pages
* `home/` – homepage hero and section images

Example reference:

```markdown
![CLEWS Workshop](/assets/images/gen/blog/clews-workshop-2025.png)
```

---

## 3.6 Layouts (`_layouts`)

Templates available include:

* `default.html`
* `post.html`
* `category.html`
* `project.html`
* `home.html`
* custom modelling layouts (e.g., `wefm.html`)

Markdown files declare layout via front matter:

```yaml
layout: post
```

---

# 4. Getting Started

## 4.1 Install Jekyll

Ensure Ruby and Jekyll are installed.
Guide: [https://jekyllrb.com/docs/installation/](https://jekyllrb.com/docs/installation/)

## 4.2 Install Dependencies

```bash
bundle install
```

## 4.3 Run the Site Locally

```bash
bundle exec jekyll serve
```

Local preview:
`http://localhost:4000`

## 4.4 Build Static Site

```bash
bundle exec jekyll build
```

Outputs to `_site/`.

---

# 5. Content Authoring Workflow

## 5.1 Create a New Post

Steps:

1. Add `.md` file in `collections/_posts/`
2. Apply correct naming convention
3. Add front matter
4. Write content
5. Push to repository

---

## 5.2 Create a New Page

Example template:

```yaml
---
layout: project
title: "New Page"
permalink: /new-page/
---
```

---

## 5.3 Add a Newsletter

1. Add PDF or `.md` file into `collections/news/`
2. Link from newsletter index page if needed

---

## 5.4 Add Images

Place in:

```
assets/images/gen/[blog|content|home]
```

---

## 5.5 Create a New Category

```yaml
---
layout: category
title: "Jordan"
category: jordan
---
```

Tag related posts:

```yaml
category: jordan
```

---

# 6. Jekyll Configuration Cheat Sheet (`_config.yml`)

```yaml
# Site identity
title: "Peace Development Fund – UN Modelling Project"
description: "Rebuilding better and greener through quantitative policy simulations."
url: "https://desa-eapd.github.io"   
baseurl: "/modelling-project"       
timezone: "UTC"
lang: "en"

# Theme
theme: jekyll-advance-pro
markdown: kramdown
highlighter: rouge

# Permalinks
permalink: /:categories/:year/:month/:day/:title/

# Collections
collections:
  posts:
    output: true
    permalink: /blog/:year/:month/:day/:title/
  news:
    output: true
    permalink: /news/:path/

# SASS
sass:
  style: compressed

# Exclusions
exclude:
  - README.md
  - Gemfile
  - Gemfile.lock
  - vendor
  - node_modules
```

---

# 7. Deployment

## 7.1 Netlify

Theme includes a working `netlify.toml`.
Guide: [https://docs.netlify.com/site-deploys/create-deploys/](https://docs.netlify.com/site-deploys/create-deploys/)

If gem installation fails: delete `Gemfile.lock`.

## 7.2 GitHub Pages

Guide: [https://jekyllrb.com/docs/github-pages/](https://jekyllrb.com/docs/github-pages/)

Project Pages require:

* `url: https://username.github.io`
* `baseurl: /repository-name`

---

# 8. Contributing

* Follow naming conventions
* Maintain clean front matter
* Use correct image locations
* Maintain consistent layouts
* Open issues for major changes

---

# 9. Credits

### Font Awesome 5 Free

[https://fontawesome.com/](https://fontawesome.com/)

### Unsplash Demo Images

[https://unsplash.com/](https://unsplash.com/)

License: [https://unsplash.com/license](https://unsplash.com/license)

```

---

If you'd like, I can now:

### ✔ Export this as a **downloadable `.md` file**  
### ✔ Add a table of contents  
### ✔ Make a more visual / branded header  
### ✔ Add GitHub workflow badges (CI/CD, pages deploy, etc.)

Just tell me.
```
