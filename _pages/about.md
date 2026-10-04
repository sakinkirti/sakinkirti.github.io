---
permalink: /
title: "Welcome to my site :)"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a Bioinformatics PhD student at UCLA interested in computational neuroscience and representation learning. In particular, I want to understand a) how the retina generates signals that are robust to varying conditions, and b) how we can use these properties in neural networks to make models robust to noise. My recent work has focused on regularizers that separate signal and nuisance variation so that models perform well on out of distribution corruptions. I'm now focused on understanding various retinal ganglion cell type functionality and what they add to visual representations.

I'm lucky to be advised by [Dr. Joel Zylberberg at UCLA](http://jzlab.org/). Prior to starting my PhD, I was fortunate to be mentored by [Dr. Patrick Ellinor at the Broad Institute](https://www.ellinorlab.org/), [Dr. Radhika Atit at Case Western Reserve University](https://case.edu/artsci/biology/atitlab/), and [Dr. Stefan Heller at Stanford](https://hellerlab-stanford.net/).

In my free time, I enjoy photography, backpacking, weightlifting, and cooking.

## Updates

{% assign news = site.data.news | sort: "date" | reverse %}
<ul class="news">
{% for item in news limit: 5 %}
  <li><span class="news__date">{{ item.date | date: "%b %Y" }}</span><span>{{ item.text | markdownify | remove: "<p>" | remove: "</p>" | strip }}</span></li>
{% endfor %}
</ul>
{% if news.size > 5 %}
<details>
  <summary>Older updates</summary>
  <ul class="news">
  {% for item in news offset: 5 %}
    <li><span class="news__date">{{ item.date | date: "%b %Y" }}</span><span>{{ item.text | markdownify | remove: "<p>" | remove: "</p>" | strip }}</span></li>
  {% endfor %}
  </ul>
</details>
{% endif %}
