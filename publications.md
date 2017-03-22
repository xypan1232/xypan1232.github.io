---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "Xiaoyong Pan, Hong-Bin Shen"
    title: "RNA-protein binding motifs mining with a new hybrid deep learning based cross-domain knowledge integration approach"
    keywords: "ideep"
    month: "November"
    year: "2016"
    address: "Copenhagen, Denmark"
    booktitle: "BMC Bioinformatics"
    url: http://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-017-1561-8

  - author: "Xiaoyong Pan, Yong-Xian Fan, Junchi Yan, Hong-Bin Shen"
    title: "IPMiner: hidden ncRNA-protein interaction sequential pattern mining with stacked autoencoder for accurate computational prediction"
    keywords: "IPMiner"
    month: "August"
    year: "2016"
    address: "Copenhagen, Denmark"
    journal: "BMC Genomics"
    url: https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-016-2931-8
---



# Publications
See my Publication at <a href="https://scholar.google.com/citations?hl=en&user=Yis2IzgAAAAJ">Google Scholar</a> <br><br>
{% for pub in page.pubs %}
{% unless pub.hidden %}
  - {% if pub.url %} [{{pub.title}}]({{pub.url}}).
    {% else %} {{pub.title}}.
    {% endif %}{% if pub.type %}({{pub.type}})
    {% endif %}<br>
    {{pub.author}}.<br>
    {% if pub.type == 'Technical Report' %}{{pub.number}}
    {% endif %}{{pub.booktitle}}{{pub.school}}{{pub.journal}}.<br>
    {% if pub.address %}{{pub.address}}.
    {% endif %} {{pub.month}}, {{pub.year}}. {% if pub.slides %}[Slides]({{pub.slides}}).
    {% endif %}{% if pub.key %}[Bibtex](http://groups.csail.mit.edu/commit/bibtex.cgi?key={{pub.key}}).
    {% endif %}{% if pub.bibtex %}[Bibtex]({{pub.bibtex}}).
    {% endif %}
{% endunless %}
{% endfor %}

#Professional Activities
Reviewer for Computational biology and chemistry, Journal of Biomedical and Health Informatics, Interdisciplinary Sciences: Computational Life Sciences.

