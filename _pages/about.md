---
permalink: /
title: "About Me"
author_profile: true
redirect_from:
- /about/
- /about.html
---

I’m Piyumal Anthony Demotte, a PhD student at [the School of Computing](https://comp.anu.edu.au/) and [the Research School of Biology](https://biology.anu.edu.au/), at [the Australian National University](https://www.anu.edu.au/). 
My work intersects with computer science and biology. My research mainly focuses on efficient algorithms and machine-learning techniques for computational biology. 
I am advised by, [A/Prof. Minh Bui](https://anu-phylogenomics.github.io/) focuses on the analysis of higher-order gene-gene interactions, molecular evolution, and dating of genetic sequences. 
I am currently an affiliated student at [the ARC Centre for Future Crop Development](https://futurecropscentre.edu.au/).

See my [CV](/cv/) for more details.


## Research Interests

I am interested in designing high-performance algorithmic techniques for phylogenomics, especially through IQ-TREE software which is widely used in phylogenomics inference.  I believe machine learning for phylogenomics and language models inspired deep learning approaches for bioinformatics could enhance our understanding of computationally expensive computational biology tasks given the data produced by next-generation sequencing.

Most recently I have been focusing on generative models, specifically normalizing flows for phylogenomics and LLMs for SNP data of plants.  My research has been exploring practical aspects of normalizing flows for computational biology.  Further, I am interested in optimizations for phylogenomic dating, software design, probabilistic programming languages, Bayesian methods, and MCMC.


# Recent News
{% include base_path %}
{% assign news = site.portfolio | reverse %}
{% assign first_post = news | first %}
{% assign first_year = first_post.date | date: '%Y' %}
{% assign first_day = first_post.date | date: '%j' %}
{% assign post_count = 0 %}
{% for post in news %}
{% assign cyear = post.date | date: '%Y' %}
{% assign cday = post.date | date: '%j' %}
{% if cyear != first_year %}
{% assign ellapsed_days = first_year | minus:cyear | times:365 | plus:first_day | minus:cday %}
{% else %}
{% assign ellapsed_days = first_day | minus:cday %}
{% endif %}

{% if ellapsed_days > 365 and post_count > 3 %}
{% break %}
{% endif %}
{% include archive-single-news.html %}
{% assign post_count = post_count | plus: 1 %}
{% endfor %}

---

For more news see [here](/news/).
