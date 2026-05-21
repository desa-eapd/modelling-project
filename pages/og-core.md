---
layout: og-core
title: "OG-Core"
permalink: "/og-core/"
description: "OG-Core is a dynamic overlapping generations model used for long-term economic projections and policy analysis."
header_transparent: false
header_color_mode: dark
meta_title: "OG-Core - United Nations Modelling Tool"

# Hero banner
hero:
  enabled: true
  heading: "OG-Core"
  sub_heading: "Dynamic overlapping-generations modelling for fiscal policy, growth, and intergenerational outcomes"
  text_color: "#FFFFFF"
  background_color: ""
  background_gradient: false
  background_image: "/assets/images/gen/home/OG-Core_V2.png"
  fullscreen_mobile: true
  fullscreen_desktop: false
  height: "750px"

# Intro section
intro:
  enabled: true
  align: left
  heading: "Understanding OG-Core"
  sub_heading: |
    Governments make fiscal decisions every year: how much to tax, how much to spend, how much to borrow, and how to allocate public resources. These choices affect households, firms, government budgets, and the broader economy not only today, but also many years into the future — hence the need for an **Overlapping Generations** (OG-Core) model to help governments & analysts study these long-term interactions.
    
    At the most basic level, fiscal policies connect three core parts of the economy: (1) **households**, who work, save, consume, and pay taxes; (2) **firms**, which hire workers, invest, and produce goods & services; and (3) **government**, which raises revenue, provides transfers & public services, and manages public debt. Because these parts interact with one another, a policy change in one area can have cascading effects across the whole economy.
    
    For example, a government may introduce a tax reform to raise revenue & improve fiscal sustainability. But that reform can also affect household savings, labour supply, or private investment. Similarly, population ageing can increase pension & health spending while reducing the share of working-age people, creating pressure on public finances and affecting future generations.
    
    OG-Core is designed to understand these interactions and capture how people & institutions respond over time. It uses an overlapping generations framework, meaning that the economy is represented by households of different ages who make decisions over their lifetimes. This makes it possible to examine how policies affect different generations, income groups, and future fiscal outcomes.

# Section: outputs and scope
overview:
  enabled: true
  align: left
  heading: "OG-Core Purpose"
  # Markdown icon list replacing the plain numbered list for visual clarity.
  sub_heading: |
        The end goal of an OG-Core assessment is to support evidence-based fiscal policy design and long-term economic planning, with roughly 4 main purposes:

        - ![Policy coherence icon](../assets/images/icons/lucide/scale.svg){: .clews-purpose-icon }

          **Fiscal sustainability:** understand how tax, spending, transfer, and debt policies affect public finances over time. For example: Is the current fiscal path sustainable? How will public debt evolve under different policy scenarios? What reforms could improve long-term fiscal balances?

        - ![Policy reform icon](../assets/images/icons/lucide/sliders-horizontal.svg){: .clews-purpose-icon }

          **Policy reform:** evaluate the macroeconomic & distributional impacts of fiscal reforms. For example: How would a change in income taxes affect labour supply & savings? How would a consumption tax reform affect households with different incomes? What are the economy-wide effects of pension or transfer reforms?

        - ![Intergenerational impacts icon](../assets/images/icons/custom/ogcore-intergenerational.svg){: .clews-purpose-icon }

          **Intergenerational impacts:** assess how policies affect different age groups & future generations. For example: Who benefits from a reform today and who bears the cost in the future? How does population ageing affect workers, retirees, and future taxpayers? How are welfare gains or losses distributed across generations?

        - ![Macroeconomic dynamics icon](../assets/images/icons/custom/ogcore-macro-dynamics.svg){: .clews-purpose-icon }

          **Macroeconomic dynamics:** analyse how fiscal policy affects growth, investment, consumption, wages, interest rates, and government revenues over time. For example: How does a tax reform affect GDP? What happens to capital accumulation & wages? How do policy choices influence long-term economic growth?
        {: .clews-purpose-list }
  buttons:
    enabled: true
    list:
      - text: "OG-Core Documentation"
        url: "https://pslmodels.github.io/OG-Core/content/intro/intro.html"
        external: true
        size: large
        style: "primary"
        
# Implementation section (5 phases rendered via icon list styles)
implementation:
  enabled: true
  band_class: "white"
  align: left
  heading: "OG-Core Implementation"
  # Markdown cards replacing the old table; all phase details are preserved.
  sub_heading: |
        To implement an OG-Core assessment, there are typically 5 phases:
        - ![Systems profiling icon](../assets/images/icons/lucide/files.svg){: .clews-phase-icon }

          **1. Policy Question & Scope**

          Define the fiscal policy issue to be analysed and set the boundaries of the assessment, including the time horizon, reform options, population groups, and macroeconomic outcomes of interest.
          
          Activities: Identify the policy question; review national fiscal priorities; define baseline and reform scenarios; determine the relevant taxes, transfers, spending categories, and demographic assumptions; engage stakeholders to clarify policy needs.

        - ![Pre-nexus assessment icon](../assets/images/icons/lucide/git-merge.svg){: .clews-phase-icon }

          **2. Data Preparation & Calibration**

          Adapt the model to the country context using available demographic, macroeconomic, fiscal, and household-level data.
          
          Activities: Compile national accounts, tax, spending, population, and labour market data; prepare household or survey data where available; calibrate model parameters; align the model baseline with observed economic and fiscal indicators.

        - ![Model development icon](../assets/images/icons/lucide/code-xml.svg){: .clews-phase-icon }

          **3. Model Development**

          Build or adapt a country-specific OG-Core application based on the policy objectives, data availability, and institutional context.
          
          Activities: Configure model parameters; develop country-specific tax and transfer functions; define government budget rules; specify demographic and productivity assumptions; validate the model baseline; prepare reform simulations.

        - ![Analysis of results icon](../assets/images/icons/lucide/chart-column.svg){: .clews-phase-icon }

          **4. Analysis of Results**

          Run baseline and reform scenarios to assess how policy changes affect households, firms, government budgets, and the overall economy over time.
          
          Activities: Simulate policy reforms; compare results against the baseline; analyse changes in GDP, investment, consumption, wages, interest rates, revenues, debt, and welfare; test sensitivities; refine assumptions where needed.

        - ![Recommendations icon](../assets/images/icons/lucide/badge-check.svg){: .clews-phase-icon }

          **5. Recommendations**

          Translate model findings into clear policy insights, highlighting fiscal trade-offs, macroeconomic effects, intergenerational impacts, and implementation considerations.
          
          Activities: Prepare charts, indicators, and scenario comparisons; identify key risks and opportunities; draft policy briefs, technical reports, presentations, and training materials; communicate findings to policymakers and stakeholders.
        {: .clews-phase-list }
  sub_heading_after: |
        If you're interested in learning more about OG-Core, take a look at our free, online course:
        {: .clews-course-note }
  buttons:
    enabled: true
    list:
      - text: "OG-Core Course"
        url: "https://capacity.desa.un.org/article/mastering-og-core-model-theory-technical-applications-and-policy-use-cases"
        external: true
        size: large
        style: "primary"

# Section: card grid for implementations
country_models:
  enabled: true
  align: left
  heading: "OG-Core in Action"
  sub_heading: "Take a look at OG-Core model implementations around the globe:"
  models:
    - name: "OG-ETH"
      country: "Ethiopia"
      flag: "/assets/images/flags/ethiopia.svg"
      description: "UN DESA implementation supporting medium- to long-term planning."
      details_url: "/og-core/ethiopia/"
      details_external: false
      repo_url: "https://github.com/EAPD-DRB/OG-ETH"
      repo_external: true
      docs_url: "/ethiopia/"
      docs_external: false
    - name: "OG-IND"
      country: "India"
      flag: "https://flagcdn.com/in.svg"
      description: "Revenue Academy implementation built on OG-Core."
      details_url: "/og-core/india/"
      details_external: false
      repo_url: "https://github.com/Revenue-Academy/OG-IND"
      repo_external: true
      docs_url: "https://revenue-academy.github.io/OG-IND/"
      docs_external: true
    - name: "OG-IDN"
      country: "Indonesia"
      flag: "https://flagcdn.com/id.svg"
      description: "UN DESA implementation used in fiscal policy dialogues."
      details_url: "/og-core/indonesia/"
      details_external: false
      repo_url: "https://github.com/EAPD-DRB/OG-IDN"
      repo_external: true
      docs_url: "/indonesia/"
      docs_external: false
    - name: "OG-MYS"
      country: "Malaysia"
      flag: "https://flagcdn.com/my.svg"
      description: "Revenue Academy implementation for Malaysian fiscal scenarios."
      details_url: "/og-core/malaysia/"
      details_external: false
      repo_url: "https://github.com/Revenue-Academy/OG-MYS"
      repo_external: true
    - name: "OG-PHL"
      country: "Philippines"
      flag: "https://flagcdn.com/ph.svg"
      description: "UN DESA implementation & training materials."
      details_url: "/og-core/philippines/"
      details_external: false
      repo_url: "https://github.com/EAPD-DRB/OG-PHL"
      repo_external: true
      docs_url: "/philippines/"
      docs_external: false
    - name: "OG-ZAF"
      country: "South Africa"
      flag: "https://flagcdn.com/za.svg"
      description: "UN DESA implementation for long-run policy simulations."
      details_url: "/og-core/south-africa/"
      details_external: false
      repo_url: "https://github.com/EAPD-DRB/OG-ZAF"
      repo_external: true
      docs_url: "/south-africa/"
      docs_external: false
    - name: "OG-UK"
      country: "United Kingdom"
      flag: "https://flagcdn.com/gb.svg"
      description: "Country calibration of OG-Core for U.K. fiscal analysis."
      details_url: "/og-core/united-kingdom/"
      details_external: false
      repo_url: "https://github.com/PSLmodels/OG-UK"
      repo_external: true
      docs_url: "https://pslmodels.github.io/OG-UK/"
      docs_external: true
    - name: "OG-USA"
      country: "United States"
      flag: "https://flagcdn.com/us.svg"
      description: "PSLmodels calibration used for U.S. policy simulations."
      details_url: "/og-core/united-states/"
      details_external: false
      repo_url: "https://github.com/PSLmodels/OG-USA"
      repo_external: true
      docs_url: "https://pslmodels.github.io/OG-USA/"
      docs_external: true
outro:
  enabled: false
---
