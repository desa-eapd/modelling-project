<h1 align="center">Peace Development Fund – UN Modelling Project</h1>

<p align="center">
  <b>Website Repository</b>
</p>

<p align="center">
  <a href="https://jekyllrb.com/"><img src="https://img.shields.io/badge/built%20with-Jekyll-red.svg" alt="Built with Jekyll"></a>
  <a href="https://www.zerostatic.io/docs/jekyll-advance/"><img src="https://img.shields.io/badge/theme-Jekyll%20Advance%20Pro-blue.svg" alt="Jekyll Advance Pro"></a>
  <a href="https://desa-eapd.github.io/modelling-project/"><img src="https://img.shields.io/badge/website-live%20site-green.svg" alt="Live Site"></a>
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
- newsletters and other knowledge products  

in a structured and accessible way for policymakers, partners, and stakeholders.

---

## **1. Project Overview**

### **Project title**

**Rebuilding better and greener from the COVID-19 pandemic through enhanced design and implementation of sustainable national recovery strategies based on policy simulations**

### **Objective**

Strengthen the capacity of government agencies to better utilize data and analytical techniques to inform strategies and decision-making processes on sustainable development through the use of quantitative modelling tools.

### **Duration**

**2023–2027**

### **Target countries**

*TBD*

### **Main activities**

- Identify planning gaps and data availability issues where enhanced modelling capacity will have the greatest impact.  
- Assess the feasibility of applying macro-economic, micro-simulation, and CLEWS integrated modelling tools in participating countries.  
- Customize modelling tools for country contexts to inform COVID-19 recovery strategies and SDG implementation.  
- Conduct national training workshops on policy simulation tools.  
- Prepare policy documents and briefs based on simulation results.  
- Support participation in regional and global policy dialogues (ECOSOC, HLPF, etc.).  
- Produce project reports, newsletters, and technical documentation.

---

## **2. Theme: Jekyll Advance Pro**

**Jekyll Advance** is a premium, multi-purpose Jekyll theme providing multiple content types, a modern semi-flat design, customizable hero sections, and responsive layouts.

- **Live demo:** <https://jekyll-advance.netlify.app/>  
- **Theme documentation:** <https://www.zerostatic.io/docs/jekyll-advance/>

The PDF Modelling Project adapts this theme to:

- Serve posts from Jekyll **collections** (`collections/_posts`)  
- Provide **categories** for country- and topic-based filtering  
- Use **pages** for core project content  
- Store **newsletters** within custom collections  
- Use `_layouts` to render Markdown content with project-specific HTML templates  

---

## **3. Repository Structure**

```text
.
├── collections/
│   ├── _posts/          # Blog/news posts and updates
│   ├── news/            # Newsletters and periodic publications
│   └── …                # Additional collections as required
│
├── pages/               # Static pages (about, project, services, countries, etc.)
│
├── categories/          # Auto-generated category/tag pages
│
├── assets/
│   └── images/
│        └── gen/
│             ├── blog/    
│             ├── content/ 
│             └── home/    
│
├── _layouts/            
│
├── _config.yml          
└── README.md
```

(Full content continues...)
