# Peace Development Fund – UN Modelling Project  
### Website Repository (Jekyll Advance Pro Theme)

This repository hosts the source code for the **Peace and Development Fund (PDF) – UN Modelling Project** website.  
The site is built with **Jekyll** using the **Jekyll Advance Pro Theme**, and is designed to present project information, country updates, modelling results, newsletters, and other knowledge products in a structured and accessible way.

---

## 1. Project Overview

### Project title

**Rebuilding better and greener from the COVID-19 pandemic through enhanced design and implementation of sustainable national recovery strategies based on policy simulations**

### Objective

Strengthen the capacity of government agencies to better utilize data and analytical techniques to inform strategies and decision-making processes on sustainable development through the use of quantitative modelling tools.

### Duration

**2023–2027**

### Target countries

*TBD*

### Main activities

- Identify planning gaps and data availability issues where enhanced modelling capacity will have the greatest impact.  
- Assess the feasibility of applying macro-economic, micro-simulation, and CLEWS integrated modelling tools in participating countries.  
- Customize modelling tools for country contexts to inform COVID-19 recovery strategies and SDG implementation.  
- Conduct national training workshops on policy simulation tools.  
- Prepare policy documents and briefs based on simulation results.  
- Support national participation in regional and global policy dialogues, including ECOSOC, HLPF, and other international fora.  
- Produce project reports, newsletters, and technical documentation.

### Key document

- Project brochure (PDF)

---

## 2. Theme: Jekyll Advance Pro

**Jekyll Advance** is a premium, multi-purpose Jekyll theme. It provides several content-types suitable for small and medium-sized organisations and project/marketing sites, with a modern semi-flat design, customizable hero images, and full-width sections.

- Live demo: <https://jekyll-advance.netlify.app/>  
- Theme documentation: <https://www.zerostatic.io/docs/jekyll-advance/>

![Jekyll Advance Theme screenshot](https://www.zerostatic.io/theme/jekyll-advance/jekyll-advance-screenshot.png)

The Peace Development Fund project adapts this theme to:

- Serve posts from Jekyll **collections** (especially `collections/_posts`)  
- Provide country- and topic-based **categories**  
- Expose **pages** for core project information  
- Store **newsletters** and media assets in dedicated folders  
- Use `_layouts` as HTML templates for the Markdown–based content.

---

## 3. Repository Structure

The sections below are the main locations content authors and maintainers will use.

```text
.
├── collections/
│   ├── _posts/          # Core blog/news posts and updates
│   ├── news/            # Newsletters and similar content
│   └── …                # Other collections if needed
│
├── pages/               # Static pages (about, home, project, services, country pages, etc.)
│
├── categories/          # Category pages used for tagging and filtering
│
├── assets/
│   └── images/
│        └── gen/
│             ├── blog/     # Blog-specific images
│             ├── content/  # General content images
│             └── home/     # Home/landing-page images
│
├── _layouts/            # HTML/Liquid templates (post, category, home, default, project, etc.)
│
├── _config.yml          # Jekyll configuration
└── README.md

3.1 Posts (collections/_posts)

Main project updates, country notes, workshop summaries, and modelling articles.

Files use the standard Jekyll naming convention: YYYY-MM-DD-title.md.

Example front matter:
---
layout: post
title: "National CLEWS Training – Philippines"
category: philippines
image: /assets/images/gen/blog/philippines-training.png
---
3.2 Pages (/pages)

Static, navigable pages such as about, about-the-project, home, services, projects, country pages (philippines, south-africa, etc.)

Each page is written in Markdown and assigned a layout from _layouts.

Example:
---
layout: project
title: "About the Modelling Project"
permalink: /about/
---
3.3 Categories (/categories)

Used exclusively for tagging and content aggregation.

For each category, there is a corresponding .md file using a category layout.

Example:
---
layout: category
title: "Philippines"
category: philippines
---
3.4 Newsletters (collections/news)

Use this folder for newsletter issues and similar periodic publications.

Files may be PDFs or Markdown (.md) with links to attachments.

3.5 Images (assets/images/gen)

blog/ – images referenced in posts.

content/ – images used inside general content and pages.

home/ – hero and section images for the home page.

Use descriptive filenames and, where possible, compressed / web-optimised images.

3.6 Layouts (/_layouts)

HTML/Liquid templates such as default.html, home.html, post.html, category.html, project.html, service.html, wefm.html, etc.

Markdown files in collections/, pages/, and categories/ specify a layout value to select one of these templates.

4. Getting Started
4.1 Prerequisites – Install Jekyll

Ensure you have Ruby and Jekyll installed.
Refer to the official Jekyll installation guide:

https://jekyllrb.com/docs/installation/

4.2 Install Dependencies

From the project root (the folder containing README.md and _config.yml):
bundle install
4.3 Run the Site Locally
bundle exec jekyll serve
# or
jekyll serve


The site will typically be served at http://localhost:4000.

4.4 Build the Site
bundle exec jekyll build


The built static site will be placed in the _site directory.

5. Content Authoring Workflow
5.1 Create a New Post

Add a file in collections/_posts/ with the name YYYY-MM-DD-title.md.

Add front matter (title, layout, category, optional image).

Write the content in Markdown.

Commit and push.

5.2 Create a New Page

Add a .md file in pages/.

Choose an appropriate layout from _layouts/.

Define the title and permalink in front matter.

Commit and push.

5.3 Add a Newsletter

Place the PDF or Markdown file in collections/news/.

If using Markdown, include front matter and link to any attachments.

Update any newsletter index page to link to the new issue (if required).

5.4 Add or Update Images

Save the file under assets/images/gen/ in the relevant subfolder (blog, content, home, etc.).

Reference it using an absolute path, for example:

![CLEWS workshop](/assets/images/gen/blog/clews-workshop-2025.png)

5.5 Define a New Category

Create a new file under categories/ (e.g. jordan.md).

Use the category layout with the appropriate title and category key.

---
layout: category
title: "Jordan"
category: jordan
---


Use category: jordan in relevant posts/pages.

6. Jekyll Configuration Cheat Sheet (_config.yml)

Below is a minimalist configuration tailored for this project. Actual values may differ in your repository; adjust as needed.

# Site identity
title: "Peace Development Fund – UN Modelling Project"
description: "Rebuilding better and greener from the COVID-19 pandemic through quantitative policy simulations."
url: "https://example.org"   # Production domain, no trailing slash
baseurl: ""                  # Set to "/repository-name" for GitHub Project Pages
timezone: "UTC"
lang: "en"

# Theme
theme: jekyll-advance-pro    # or remote_theme: "zerostatic/jekyll-advance"

markdown: kramdown
highlighter: rouge

# Permalinks for posts
permalink: /:categories/:year/:month/:day/:title/

# Collections (example)
collections:
  posts:
    output: true
    permalink: /blog/:year/:month/:day/:title/
  news:
    output: true
    permalink: /news/:path/

# Sass/CSS
sass:
  style: compressed

# Excluded files from build
exclude:
  - README.md
  - node_modules
  - vendor
  - Gemfile
  - Gemfile.lock


Key points:

For a GitHub Project site, set:

url: "https://username.github.io"

baseurl: "/repository-name"

For a root domain deployment, keep baseurl: "".

7. Deployment
7.1 Netlify

The theme ships with a netlify.toml file that configures a standard Jekyll build.
Netlify documentation for site creation and deployment:

https://docs.netlify.com/site-deploys/create-deploys/

If bundle installation fails on Netlify, deleting Gemfile.lock and redeploying can sometimes resolve version conflicts.

7.2 GitHub Pages

The theme is tested with GitHub Pages.
See the Jekyll documentation:

https://jekyllrb.com/docs/github-pages/

For GitHub Project Pages (https://username.github.io/repository):

Set url to https://username.github.io.

Set baseurl to /repository.

Ensure asset paths in templates and content use {{ site.baseurl }} where appropriate.

8. Contributing

When contributing to this repository:

Follow the naming conventions for posts (YYYY-MM-DD-title.md).

Use consistent front matter for posts, pages, and categories.

Store images in the appropriate assets/images/gen/ subfolder.

Reuse existing layouts where possible to maintain visual consistency.

For significant structural or design changes, open an issue and/or submit a pull request describing the proposed change.

9. Credits

This project uses the Jekyll Advance Pro Theme and several open-source assets.

Font Awesome 5 Free

Project: https://fontawesome.com/

License: https://fontawesome.com/license/free

Demo content images

Unsplash: https://unsplash.com/

License: https://unsplash.com/license



