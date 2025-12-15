# Peace Development Fund – UN Modelling Project

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

The site is built with **Jekyll** using the **Jekyll Advance Pro Theme**, and is designed to present structured project information, modelling updates, newsletters, and knowledge products.

---

## 1. Project Overview

### Project Title
Rebuilding better and greener from the COVID-19 pandemic through enhanced design and implementation of sustainable national recovery strategies based on policy simulations

### Objective
Strengthen the capacity of government agencies to use quantitative modelling tools to inform sustainable development strategies.

### Duration
2023–2027

### Target Countries
TBD

### Main Activities
- Identify planning and data gaps  
- Assess modelling feasibility (macro, micro, CLEWS)  
- Conduct capacity-building and workshops  
- Develop country modelling outputs  
- Produce briefs and technical documents  
- Support global policy dialogue participation  

---

## 2. Theme: Jekyll Advance Pro

Jekyll Advance Pro is a premium multi-purpose Jekyll theme.

- Live Demo: https://jekyll-advance.netlify.app/  
- Documentation: https://www.zerostatic.io/docs/jekyll-advance/

The project uses the theme for:

- Collections-based posts  
- Category-based filtering  
- Structured page layouts  
- Newsletter integration  
- Custom Liquid layouts  

---

## 3. Repository Structure

```text
.
├── collections/
│   ├── _posts/
│   ├── news/
│
├── pages/
├── categories/
├── assets/
│   └── images/gen/
│        ├── blog/
│        ├── content/
│        └── home/
├── _layouts/
├── _config.yml
└── README.md
```

---

## 4. Content Authoring Workflow

### Posts (`collections/_posts`)
Format:

```
YYYY-MM-DD-title.md
```

Example:

```yaml
---
layout: post
title: "National CLEWS Training – Philippines"
category: philippines
image: /assets/images/gen/blog/philippines-training.png
---
```

### Pages (`pages/`)

```yaml
---
layout: project
title: "About the Modelling Project"
permalink: /about/
---
```

### Categories (`categories/`)

```yaml
---
layout: category
title: "Philippines"
category: philippines
---
```

### Newsletters (`collections/news`)
PDF or Markdown.

### Images (`assets/images/gen`)
Referenced as:

```markdown
![CLEWS](/assets/images/gen/blog/clews.png)
```

### Layouts (`_layouts`)
Templates include:
- post.html  
- category.html  
- project.html  
- home.html  

---

## 5. Getting Started

### Install Jekyll
https://jekyllrb.com/docs/installation/

### Install dependencies

```bash
bundle install
```

### Run locally

```bash
bundle exec jekyll serve
```

### Build static site

```bash
bundle exec jekyll build
```

---

## 6. Jekyll Configuration Cheat Sheet

```yaml
title: "Peace Development Fund – UN Modelling Project"
description: "Rebuilding better and greener through quantitative policy simulations."
url: "https://desa-eapd.github.io"
baseurl: "/modelling-project"
timezone: "UTC"
lang: "en"

theme: jekyll-advance-pro

markdown: kramdown
highlighter: rouge

permalink: /:categories/:year/:month/:day/:title/

collections:
  posts:
    output: true
    permalink: /blog/:year/:month/:day/:title/
  news:
    output: true
    permalink: /news/:path/

sass:
  style: compressed

exclude:
  - README.md
  - Gemfile
  - Gemfile.lock
  - vendor
  - node_modules
```

---

## 7. Deployment

### Netlify  
Use `netlify.toml`.  
Guide: https://docs.netlify.com/site-deploys/create-deploys/

### GitHub Pages  
Guide: https://jekyllrb.com/docs/github-pages/

---

## 8. Contributing

- Follow naming conventions  
- Maintain clean front matter  
- Store images correctly  
- Reuse layouts  
- PR major changes  

---

## 9. Credits

### Font Awesome  
https://fontawesome.com/

### Unsplash Images  
https://unsplash.com/  
License: https://unsplash.com/license
