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
    <h1 class="about-hero__title">Tanxin (Casey) Liu</h1>
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
- *2026.05*: Our preprint on RAG-mediated structural variation and relapse risk in acute lymphoblastic leukemia is out on medRxiv.
- *2025.08*: I passed my qualifying exam.

<span class='anchor' id='publications'></span>
# Selected Publications

<div class="publication-stack">
  <article class="publication-card">
    <h3><a href="https://doi.org/10.64898/2026.05.21.26353542">RAG-mediated structural variation and its impact on relapse risk in acute lymphoblastic leukemia</a></h3>
    <p class="publication-card__badge">medRxiv preprint, 2026</p>
    <p class="publication-card__authors"><strong>Tanxin Liu</strong>, Yaqi Li, Chenxi Wang, Cameron J. Clark, Nathan Anderson, Erin Marcotte, Michael R. Lieber, Suchitra Swaminathan, Joseph L. Wiemels, Logan G. Spector, Vijay G. Sankaran, Charles Fries, Adam J. de Smith</p>
    <ul>
      <li>Led the analysis of RAG-mediated structural variants and relapse risk in a childhood B-ALL cohort, integrating WES, WGS, and RNA-seq with MRD status, survival, and time-to-relapse.</li>
      <li>Established an association with relapse in survival models, including among MRD-negative patients.</li>
    </ul>
  </article>

  <article class="publication-card">
    <h3><a href="https://www.nature.com/articles/s41375-024-02407-3">Early-life tobacco exposure is causally implicated in aberrant RAG-mediated recombination in childhood acute lymphoblastic leukemia</a></h3>
    <p class="publication-card__badge">Leukemia, 2024</p>
    <p class="publication-card__authors"><strong>Tanxin Liu</strong>, Keren Xu, Anmol Pardeshi, Swe Swe Myint, Alice Y. Kang, Libby M. Morimoto, Michael R. Lieber, Joseph L. Wiemels, Scott C. Kogan, Catherine Metayer, Adam J. de Smith</p>
    <ul>
      <li>Developed bioinformatics pipelines for somatic variants (SNV/indels/structural variants/copy number alterations) discovery and identified driver mutations and secondary genetic events in childhood acute lymphoblastic leukemia patients using whole‑genome sequencing data of paired tumor‑normal samples on high‑performance computing cluster.</li>
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

  <article class="publication-card">
    <h3>Single-cell multiomic mapping of genetic predisposition to childhood B-cell acute lymphoblastic leukemia</h3>
    <p class="publication-card__badge">Submitted to Cancer Discovery, 2026</p>
    <p class="publication-card__authors">Alexander J. Lee, Anna-Lena Neehus, Lara Wahlster, Gaurav Agarwal, Chunyan Weng, Aoi Zhang, <strong>Tanxin Liu</strong>, Samuel Shelton, Tian Ye, Leonardo della Volpe, Ofir Cohn, Mark Poeschla, Elizabeth King, Seung-Ah Ha, Alexander Turvey, Adam J. de Smith, Vijay G. Sankaran</p>
  </article>

  <article class="publication-card">
    <h3>A functional genomics screen of human B-cell differentiation reveals convergent mechanisms of inherited childhood leukemia predisposition</h3>
    <p class="publication-card__badge">Manuscript in preparation, 2026</p>
    <p class="publication-card__authors">Lara Wahlster, Anna-Lena Neehus, Alexander J. Lee, Sanchi Mazumder, Parisa Mehrzad, Sarah Black, Letizia Messa, <strong>Tanxin Liu</strong>, Chunyan Weng, Alexis Caulier, Joshua Pak, Travis Fleming, Mateusz Antoszewski, Aoi Zhang, Seung-Ah Ha, Adam J. de Smith, Vijay G. Sankaran</p>
  </article>

  <article class="publication-card">
    <h3><a href="https://doi.org/10.1002/ijc.34624">External validation of genetically predicted protein biomarkers for pancreatic cancer risk using aptamer-based plasma levels: a prospective analysis in the Atherosclerosis Risk in Communities (ARIC) Study</a></h3>
    <p class="publication-card__badge">International Journal of Cancer, 2023</p>
    <p class="publication-card__authors"><strong>Tanxin Liu</strong>, Corinne E. Joshu, Jiayun Lu, Anna Prizment, Nilanjan Chatterjee, Josef Coresh, Lang Wu, Elizabeth A. Platz</p>
    <ul>
      <li>Conducted proteomics analyses of genetically predicted protein biomarkers using aptamer-based plasma levels in a prospective cohort.</li>
    </ul>
  </article>

  <article class="publication-card">
    <h3><a href="https://doi.org/10.1093/gigascience/giae012">Proteome-wide association study and functional validation identify novel protein markers for pancreatic ductal adenocarcinoma</a></h3>
    <p class="publication-card__badge">GigaScience, 2024</p>
    <p class="publication-card__authors">Jingjing Zhu, Ke Wu, Shuai Liu, Alexandra Masca, Hua Zhong, Tai Yang, Dalia H. Ghoneim, Praveen Surendran, <strong>Tanxin Liu</strong>, Qizhi Yao, Tao Liu, Sarah Fahle, Adam Butterworth, Md A. Alam, Jaydutt V. Vadgama, Youping Deng, Hong-Wen Deng, Chong Wu, Yong Wu, Lang Wu</p>
  </article>
</div>

<p class="publication-more">More publications on my <a href="https://scholar.google.com/citations?user=Ge5lH_kAAAAJ&hl=en">Google Scholar profile</a>.</p>

<span class='anchor' id='honors-and-awards'></span>
# Honors and Awards
- *2020.07*: Peking University Best Thesis Award

<span class='anchor' id='experience'></span>
# Experience
- *2022 - present*: **Pre-Doctoral Research Fellow**, Center for Genetic Epidemiology, University of Southern California — Los Angeles, CA.
- *2020 - 2022*: **Statistical Programmer**, Johns Hopkins Medicine and Johns Hopkins Bloomberg School of Public Health — Baltimore, MD.

<span class='anchor' id='education'></span>
# Education
- *2022.08 - present*: PhD in Genetic Epidemiology (Bioinformatics track), Keck School of Medicine, University of Southern California. GPA 3.72/4.0.
- *2025*: Master of Science in Computer Science, Georgia Institute of Technology. GPA 3.9/4.0.
- *2020.08 - 2022.05*: Master of Health Science in Epidemiology, Johns Hopkins Bloomberg School of Public Health. GPA 4.0/4.0.
- *2015.09 - 2020.07*: Bachelor of Biomedicine, Minor in Psychology and Cognitive Science, Peking University Health Science Center.

<span class='anchor' id='invited-talks'></span>
# Talks and Presentations
- *2024.12*: 66th American Society of Hematology Annual Meeting and Exposition. Oral presentation, Session 614: Genomic Determinants of Outcomes in ALL.
- *2024 Spring*: Center for Genetic Epidemiology, University of Southern California. Somatic tumor mutations and environmental modifiers in childhood acute lymphoblastic leukemia patients.

<span class='anchor' id='skills'></span>
# Skills
- **Bioinformatics**: GATK, TCGA, GDC, SAMtools, PLINK, BioPython, Snakemake, Mamba, Conda, Bioconductor, AWS, Singularity, Docker.
- **Machine learning**: deep learning, classical machine learning, variational inference, object-oriented programming.
- **Programming**: Python, R, Snakemake, Linux/Unix, SAS, C++, Java.