---
permalink: /
title: "About Me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a first-year PhD candidate at the HKUST NLP Group, supervised by Professor Junxian He. I graduated from Shanghai Jiao Tong University (SJTU) in June 2024.

My research focuses on natural language processing and machine learning, with specific interests in:
- LLM Reasoning and Reinforcement Learning
- Hallucination in Vision-Language Models (VLM)
- LLM truthfulness and Interpretability

## Education

- **Ph.D. in Computer Science** (2024–Present), Hong Kong University of Science and Technology
- **B.Eng.** (2020–2024), Shanghai Jiao Tong University

## Research Experience

- **Research Intern** (February 2025 – Present), MINIMAX
- **Research Intern** (June 2024 – September 2024), Tencent WXG, advised by Zifei Shan
- **Research Intern** (June 2023 – December 2023), Shanghai AI Lab, advised by Prof. Yu Cheng

## Selected Publications

See the [publications page](/publications/) for the full list.

<ul>
{% for pub in site.publications reversed %}
  <li>
    {{ pub.authors | markdownify | remove: '&lt;p&gt;' | remove: '&lt;/p&gt;' }}
    ({{ pub.venue }}, {{ pub.year }})
    <em>{{ pub.title }}</em>
    {% if pub.content != "" %}
      <br /><small>{{ pub.content | strip_html }}</small>
    {% endif %}
  </li>
  {% if forloop.index == 6 %}
    {% break %}
  {% endif %}
{% endfor %}
</ul>

## Awards

- Zhiyuan Honor Scholarship, Shanghai Jiao Tong University
