---
layout: page
permalink: /publications/index.html
title: Publications
pubs:
  - author: "Xiaoyong Pan*, Hong-Bin Shen*"
    title: "RNA-protein binding motifs mining with a new hybrid deep learning based cross-domain knowledge integration approach"
    keywords: "ideep"
    month: "November"
    year: "2017"
    address: "Copenhagen, Denmark"
    booktitle: "BMC Bioinformatics"
    url: http://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-017-1561-8
	
  - author: "Alexander Junge, Jan C. Refsgaard, Christian Garde, Xiaoyong Pan, Alberto Santos, Ferhat Alkan, Christian Anthon, Christian von Mering, Christopher T. Workman, Lars Juhl Jensen, and Jan Gorodkin"
    title: "RAIN: RNA-protein Association and Interaction Networks."
    keywords: "RAIN"
    month: "Jan"
    year: "2017"
    address: "Copenhagen, Denmark"
    booktitle: "Database (Oxford)"
    url: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5225963/
	
  - author: "Xiaoyong Pan, Yong-Xian Fan, Junchi Yan, Hong-Bin Shen"
    title: "IPMiner: hidden ncRNA-protein interaction sequential pattern mining with stacked autoencoder for accurate computational prediction"
    keywords: "IPMiner"
    month: "August"
    year: "2016"
    address: "Copenhagen, Denmark"
    journal: "BMC Genomics"
    url: https://bmcgenomics.biomedcentral.com/articles/10.1186/s12864-016-2931-8

  - author: "Xiaoyong Pan, Hong-Bin Shen"	
    title: "OUGENE: a disease associated over-expressed and under-expressed gene database"
    keywords: "OUGENE"
    month: "May"
    year: "2016"
    address: "Copenhagen, Denmark"
    journal: "Science Bulletin"
    url: http://www.sciencedirect.com/science/article/pii/S2095927316301189
	
- author: "Xiaoyong Pan*, Kai Xiong"	
    title: "PredcircRNA: computational classification of circular RNA from other long non-coding RNA using hybrid features"
    keywords: "PredcircRNA"
    month: "May"
    year: "2015"
    address: "Copenhagen, Denmark"
    journal: "Molecular BioSystems"
    url: http://pubs.rsc.org/-/content/articlelanding/2015/mb/c5mb00214a#!divAbstract
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

