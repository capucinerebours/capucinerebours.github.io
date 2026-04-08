---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
You can also find my articles on my [Google Scholar profile]({{ site.author.googlescholar }}).
{% endif %}

{% include base_path %}

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}
        {% continue %}
      {% endif %}
      {% unless title_shown %}
## {{ category[1].title }}
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

## Conference Presentations

**Rebours, C., & Kruck, J.** (April 2026). Predictors of autistic burnout severity in autistic adults: roles of gender, camouflaging, and executive functioning. *International Society for Autism Research Annual Meeting*. Prague, Czech Republic.

**Rebours, C., & Kruck, J.** (October 2025). Risk Factors and Recovery Strategies in Autistic Burnout: A Qualitative Analysis. *National Conference on Clinical Neuropsychology*. Lille, France.

**Rebours, C., & Kruck, J.** (July 2025). Risk and Recovery Factors in Autistic Burnout: What Are the Vulnerabilities Faced by Autistic Women? *Conference of the French Association of Psychology and Health (AFPSA)*. Toulouse, France.

**Rebours, C., & Kruck, J.** (October 2024). Autistic Burnout: An Invisible Vulnerability in Autistic Women and Gender Minorities? *Université d'Automne de l'ARAPI*. Le Croisic, France.