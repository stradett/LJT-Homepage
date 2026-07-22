---
permalink: /
title: "Junteng Liu"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Junteng Liu is a first-year PhD candidate at the HKUST NLP Group, Hong Kong University of Science and Technology, where he is advised by Professor Junxian He. His research focuses on natural language processing and machine learning.

Education
======
* Ph.D. in Computer Science, Hong Kong University of Science and Technology, 2024--Present
* B.Eng., Shanghai Jiao Tong University, 2020--2024 (graduated June 2024)

Research Experience
======
* Research Intern, MINIMAX, February 2025--Present
* Research Intern, Tencent WXG, June 2024--September 2024
* Research Intern, Shanghai AI Lab, June 2023--December 2023

Research Interests
======
* LLM Reasoning and Reinforcement Learning
* Hallucination in Vision-Language Models (VLM)
* LLM Truthfulness and Interpretability

Publications
======
{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category  %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
        <h2>{{ category[1].title }}</h2><hr />
        {% assign title_shown = true %}
      {% endunless %}
      {% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
    {% include archive-single.html %}
  {% endfor %}
{% endif %}

Awards
======
* Zhiyuan Honor Scholarship, Shanghai Jiao Tong University

Contact
======
* Email: [jliugi@connect.ust.hk](mailto:jliugi@connect.ust.hk)
* GitHub: [Vicent0205](https://github.com/Vicent0205)
* Google Scholar: [Profile](https://scholar.google.com/citations?hl=en&user=tbK9jl4AAAAJ&view_op=list_works&sortby=pubdate)
* X (Twitter): [@junteng88716710](https://twitter.com/junteng88716710)
