---
permalink: /
title: "Quang-Binh Nguyen"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

# About Me

I am a Research Resident at Qualcomm AI Research, advised by Dr. Khoi Nguyen. I obtained my Bachelor's Degree in Computer Science - Honors Program at University of Science, VNU-HCM, under the supervision of Prof. Minh-Triet Tran and Dr. Trung-Nghia Le.

My research focuses on controllable image generation, particularly image personalization (diffusion and autoregressive models). Recently, I have been working on test-time alignment for generative models.

Feel free to reach out via [email](mailto:chnguyen032005@gmail.com) or [LinkedIn](https://www.linkedin.com/in/hoang-nguyen-cao/) if you'd like to connect!

---

# Experience

{% if site.work_experience %}
<div class="archive--card-grid">
  {% for post in site.work_experience reversed %}
    {% include archive-single.html type="card" %}
  {% endfor %}
</div>
{% endif %}

---

# Publications

{% if site.publications %}
<div class="archive--card-grid">
  {% for post in site.publications reversed %}
    {% include archive-single.html type="card" %}
  {% endfor %}
</div>
{% endif %}

---

# Projects

{% if site.portfolio %}
<div class="archive--card-grid">
  {% for post in site.portfolio reversed %}
    {% include archive-single.html type="card" %}
  {% endfor %}
</div>
{% endif %}

---

# Achievements

{% if site.achievements %}
<div class="archive--card-grid">
  {% for post in site.achievements reversed %}
    {% include archive-single.html type="card" %}
  {% endfor %}
</div>
{% endif %}
 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
