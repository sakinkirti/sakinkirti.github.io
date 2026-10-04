---
layout: archive
title: "Curriculum Vitae"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education
__PhD, Bioinformatics__ | University of California, Los Angeles / Los Angeles, CA<br>
Sep 2025 - Present

__BA, Computer Science__ | Case Western Reserve University / Cleveland, OH<br>
Aug 2019 - May 2023

## Experience
__Computational Associate__ | The Broad Institute of MIT and Harvard / Cambridge, MA<br>
Jul 2023 - Jul 2025<br>
_Computer Vision, Drug Discovery, Representation Learning, Cardiovascular Disease, Google Cloud Platform_

__Junior Machine Learning Engineer__ | Trustlogix / Mountain View, CA<br>
Nov 2023 - Jan 2024<br>
_Large Language Models, Database Security, Agentic Workflows, Amazon Web Services_

__Undergraduate Researcher__ | Case Western Reserve University / Cleveland, OH<br>
Nov 2019 - May 2023<br>
_Beckman Scholars Program, Computer Vision, Image Pipeline Development, Cell Shape Analysis, Applied Machine Learning_

__Undergraduate Researcher__ | Center for Computational Imaging and Personalized Diagnostics / Cleveland, OH<br>
Jan 2022 - Oct 2022<br>
_Research Ethics, Convolutional Neural Networks, High Performance Computing_

__Machine Learning Engineer Intern__ | Surgo Ventures / Washington, DC<br>
Jun 2022 - Aug 2022<br>
_Bayesian Networks, Probabilistic Models, Amazon Web Services, R, Python, Regression Models_

__Data Engineering Intern__ | Edifice Analytics / Cleveland, OH<br>
Aug 2021 - Dec 2021<br>
_Applied Machine Learning, Hadoop, Apache Spark_

__Research Intern__ | Stanford University School of Medicine / Stanford, CA<br>
Aug 2018 - Aug 2019<br>
_in-situ hybridizations, scRNA-seq_

## Funding
__Beckman Scholar's Program__ | Arnold and Mabel Beckman Foundation & Case Western Reserve University<br>
May 2020 - Aug 2021<br>
_$21,000 research grant supporting undergraduate research projects_

## Honors and Awards
__Junior-Senior Scholarship__ | Case Alumni Association<br>
Aug 2021 - May 2023<br>
_$2,000 award for students with professional promise_

__Highest Achieving Sophomore__ | Case Western Reserve University<br>
May 2020<br>
_Maintaining GPA of 4.0 through first two years_

__University Scholarship__ | Case Western Reserve University<br>
Aug 2019 - May 2023<br>
_$80,000 merit-based scholarship_

__Best Undergraduate Poster__ | Society for Developmental Biology<br>
Oct 2019<br>
_Exceptional poster presentation at SDB regional conference_

__Dean's High Honors__ | Case Western Reserve University<br>
Dec 2019 - May 2023<br>
_Maintaining GPA > 3.75_

## Teaching
__Teaching Assistant__ | Dr. Vipin Chaudhary<br>
Apr 2023 - May 2023<br>
_Introduction to Machine Learning for Industry Professionals_
  
## Publications
<ul class="cv-list">
{% assign cv_publications = site.publications | sort: "date" | reverse %}
{% for post in cv_publications %}
  <li>{{ post.citation | replace: "S Kirti", "<strong>S Kirti</strong>" }}</li>
{% endfor %}
</ul>

## Talks
<ul class="cv-list">
{% assign cv_talks = site.talks | sort: "date" | reverse %}
{% for post in cv_talks %}
  <li>{{ post.type }}: {{ post.title }}, {{ post.venue }}, {{ post.location }} · {{ post.date | date: "%b %Y" }}</li>
{% endfor %}
</ul>
