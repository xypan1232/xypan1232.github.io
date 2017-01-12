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
    booktitle: "biorxiv"
    url: http://biorxiv.org/content/early/2016/11/03/085191

---

# Publications

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



