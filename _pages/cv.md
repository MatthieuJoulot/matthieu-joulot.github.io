---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* PhD, Sorbonne Université, Paris — *2024 – present*
* Diplôme d'ingénieur, Telecom Physique Strasbourg — *2017 – 2020*
* Classes préparatoires aux grandes écoles, Chaptal, Paris — *2016 – 2017*
* Baccalauréat Scientifique, Saint Michel de Picpus, Paris — *2015*

Work experience
======
* **PhD student** — Paris Brain Institute, Aramis Lab *(Mar. 2024 – present)*
  * Supervisors: Ninon Burgos, Olivier Colliot
  * Thesis: Longitudinal processing of neuroimages for the study of neurodegenerative diseases
  * Keywords: longitudinal, processing, registration, segmentation, brain MRI, benchmark

* **Medical Imaging Research Engineer** — Paris Brain Institute, Aramis Lab *(Jun. 2021 – Mar. 2024)*
  * Development of [Clinica](https://www.clinica.run/), an open-source neuroimaging platform
  * BIDS standardisation of neuroimaging datasets
  * Refactoring of image processing pipelines (Nipype, Pydra)
  * Collaborations with FrontLab (GENFI dataset) and AlzheimerCentrum Amsterdam

* **Research Engineer** — SunLeaderSide Consulting, Caen *(2020 – 2021)*
  * Designed and built an ophthalmic measurement software
  * Patent: *Method for determining metrological parameters of an individual with a pair of spectacles* ([WO2022189147](https://patentscope.wipo.int/search/en/detail.jsf?docId=WO2022189147))

Skills
======
* **Neuroimaging tools:** FreeSurfer, FSL, ANTs, SPM, MRtrix, Nipype, Pydra, Nibabel, Nilearn
* **Programming:** Python, SLURM, Bash, Matlab, Java, C++, LaTeX
* **DevOps:** GitHub, Docker, DVC
* **Languages:** French (native), English (professional)

Publications
======

* **First author**
{% assign first_cats = "manuscripts_first,conferences_first,abstracts_first" | split: "," %}
{% for cat_key in first_cats %}
  {% assign cat_posts = site.publications | where: "category", cat_key %}
  {% if cat_posts.size > 0 %}
  * {{ site.publication_category[cat_key].title }}: {{ cat_posts.size }}
  {% endif %}
{% endfor %}
* **Co-author**
{% assign co_cats = "manuscripts_co,conferences_co,abstracts_co" | split: "," %}
{% for cat_key in co_cats %}
  {% assign cat_posts = site.publications | where: "category", cat_key %}
  {% if cat_posts.size > 0 %}
  * {{ site.publication_category[cat_key].title }}: {{ cat_posts.size }}
  {% endif %}
{% endfor %}

[See full list of publications →](/publications/)

Software
======
* **[Clinica](https://github.com/aramis-lab/clinica)** — Open-source software platform for clinical neuroimaging research. Development of new functionalities, software maintenance, user support.

Other activities
======
* **Peer review** — Computer Methods and Programs in Biomedicine
* **Organisation** — MIDL 2024 doctoral symposium (Medical Imaging with Deep Learning, Paris)
* **Instructor** — Neuro OpenScience Workshop (NOW) 2023, Paris Brain Institute: hands-on tutorial on code and data versioning
* **Participation** — OHBM Brainhack 2022 & 2023
* **Member** — Ajités (Paris Brain Institute's association of young researchers): organisation of Professional Breakfasts (2021–2022) and monthly Happy Hour (2022–2024)
