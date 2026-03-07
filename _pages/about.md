---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

<section class="about-hero">
  <div class="about-hero__content">
    <p class="about-hero__kicker">Precision Medicine | Population Health</p>
    <h1 class="about-hero__title">Tanxin (Tracy) Liu</h1>
    <p class="about-hero__subtitle">PhD Candidate in Epidemiology, Keck School of Medicine, University of Southern California</p>
    <p class="about-hero__intro">
      I focus on variant discovery in human DNA sequencing data and genome-wide association analyses to better understand inherited and somatic risk factors of childhood hematological malignancies, especially acute lymphoblastic leukemia.
    </p>
    <div class="about-hero__tags">
      <span>Whole-Genome Sequencing</span>
      <span>GWAS and Fine-Mapping</span>
      <span>Somatic Structural Variation</span>
      <span>Computational Oncology</span>
    </div>
  </div>
</section>

<section class="about-pillar-grid">
  <article class="about-pillar-card">
    <img src="/images/motif.png" alt="Bioinformatics illustration" loading="lazy" />
    <div class="about-pillar-card__body">
      <h3>Bioinformatics</h3>
      <p>I build high-throughput and reproducible computational pipelines for large genomic cohorts, from variant calling to integrative multi-omics analysis.</p>
    </div>
  </article>

  <article class="about-pillar-card">
    <img src="/images/Manhattan_Plot.png" alt="Genetic epidemiology Manhattan plot" loading="lazy" />
    <div class="about-pillar-card__body">
      <h3>Genetic Epidemiology</h3>
      <p>I perform population-level analyses, risk modeling, and cross-cohort inference to uncover disease patterns and quantify genetic and environmental determinants.</p>
    </div>
  </article>

  <article class="about-pillar-card">
    <img src="/images/pillar-cancer-genomics-cool.svg" alt="Acute lymphoblastic leukemia lineage diagram illustration" loading="lazy" />
    <div class="about-pillar-card__body">
      <h3>Cancer Genomics</h3>
      <p>I investigate somatic evolution and structural variation in hematological malignancies to connect genomic signatures with clinically meaningful biology.</p>
    </div>
  </article>
</section>

<section class="about-focus-panel">
  <h2>Current Focus</h2>
  <ul>
    <li>Decoding mutational processes and structural variation mechanisms in childhood ALL.</li>
    <li>Integrating sequencing and population-genetic evidence to prioritize candidate risk variants.</li>
    <li>Translating computational findings into clinically meaningful biomarkers.</li>
  </ul>
</section>

{% comment %}
I have published more than 17 papers at the top journal with total <a href='https://scholar.google.com/citations?user=Ge5lH_kAAAAJ'>google scholar citations <strong><span id='total_cit'>260000+</span></strong></a> (You can also use google scholar badge <a href='https://scholar.google.com/citations?user=Ge5lH_kAAAAJ'><img src="https://img.shields.io/endpoint?url={{ url | url_encode }}&logo=Google%20Scholar&labelColor=f6f6f6&color=9cf&style=flat&label=citations"></a>).
{% endcomment %}

<span class='anchor' id='news'></span>
# News
- *2025.08*: I passed my qualifying exam.

<span class='anchor' id='publications'></span>
# Selected Publications

<div class="publication-stack">
  <article class="publication-card">
    <h3><a href="https://www.nature.com/articles/s41375-024-02407-3">V(D)J recombination, somatic structural variation and environmental modifiers in childhood acute lymphoblastic leukemia</a></h3>
    <p class="publication-card__authors"><strong>Tanxin Liu</strong>, Keren Xu, Anmol Pardeshi, Swe Swe Myint, Alice Y. Kang, Libby M. Morimoto, Michael R. Lieber, Joseph L. Wiemels, Scott C. Kogan, Catherine Metayer, Adam J. de Smith</p>
    <ul>
      <li>Built pipelines for somatic variant discovery and identified driver mutations from 30+ TB paired tumor-normal whole-genome sequencing data.</li>
      <li>Conducted motif enrichment and de novo motif scanning around deletion breakpoints in immune receptor regions.</li>
      <li>Performed mutational signature analysis with matrix-factorization-based methods.</li>
    </ul>
  </article>

  <article class="publication-card">
    <h3><a href="https://www.sciencedirect.com/science/article/pii/S0006497124030647">Genome-wide association study of acute lymphoblastic leukemia in Hispanic/Latino children identifies a putatively novel risk locus at chromosome 5q31.1</a></h3>
    <p class="publication-card__badge">ASH Talk 2024</p>
    <p class="publication-card__authors"><strong>Tanxin Liu</strong>, Jalen Langie, Wenjian Yang, Libby Morimoto, Xiaomei Ma, Catherine Metayer, Philip J. Lupo, Michael E. Scheurer, Jun J. Yang, Joseph L. Wiemels, Charleston W.K. Chiang, Adam J. de Smith</p>
    <ul>
      <li>Led GWAS meta-analyses, conditional analyses, and fine-mapping for childhood ALL in admixed American populations.</li>
      <li>Constructed and validated polygenic risk scores for childhood cancer susceptibility and blood cell traits.</li>
    </ul>
  </article>

  <article class="publication-card">
    <h3>The landscape and epidemiology of somatic RAG-mediated deletions in childhood acute lymphoblastic leukemia</h3>
    <p class="publication-card__badge">Coming soon (draft completed)</p>
    <ul>
      <li>Performed population-scale analyses of RAG-mediated structural variation using whole-genome sequencing data.</li>
      <li>Characterized somatic structural-variant landscapes across childhood cancer cohorts.</li>
      <li>Investigated potential allelic-imbalance mechanisms.</li>
    </ul>
  </article>

  <article class="publication-card">
    <h3><a href="https://www.sciencedirect.com/science/article/pii/S0006497125061154">Backtracking the cellular origins of ETV6::RUNX1 childhood acute lymphoblastic leukemia in cord blood (ReCord study)</a></h3>
    <p class="publication-card__authors">Adam de Smith, Natalina Elliott, Amiya Tucker, <strong>Tanxin Liu</strong>, Nawara Ahsan, Adam Mead, Irene Roberts, Joseph Wiemels, Michelle Roesler, Logan Spector, Anindita Roy</p>
    <ul>
      <li>Developed robust pipelines for somatic variant and structural-variant discovery.</li>
      <li>Built Snakemake workflows for bulk RNA-seq, RNAseqCNV, and gene fusion detection in pediatric leukemia samples.</li>
      <li>Developed long-read analysis pipelines and applied machine learning methods for leukemia subtype classification.</li>
    </ul>
  </article>
</div>

<span class='anchor' id='honors-and-awards'></span>
# Honors and Awards
- *2020.07*: Peking University Best Thesis Award

<span class='anchor' id='education'></span>
# Education
- *2022.08 - present*: PhD candidate in Genetic Epidemiology, University of Southern California.
- *2020.08 - 2022.05*: Master of Health Science in Epidemiology, Johns Hopkins University.
- *2015.09 - 2020.07*: Bachelor of Biomedicine, Minor in Psychology, Peking University Health Science Center.

<span class='anchor' id='invited-talks'></span>
# Invited Talks
- *2024.12*: 66th American Society of Hematology Annual Meeting and Exposition. Session 614: Genomic Determinants of Outcomes in ALL.

<span class='anchor' id='internships'></span>
# Internships
- To be updated.