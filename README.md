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
