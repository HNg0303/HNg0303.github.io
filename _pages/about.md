---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

# About Me

I am a third-year student of the APCS (Advanced Program In Computer Science) at University of Science, Vietnam National University Ho Chi Minh City. I am currently an Undergraduate Researcher under the direct supervision of [Dr. Trung-Nghia Le](https://ltnghia.github.io/).

My research focuses on VLMs in cross-modal retrieval and controllable image generation. 

Feel free to reach out via [email](mailto:chnguyen032005@gmail.com) or [LinkedIn](https://www.linkedin.com/in/hoang-nguyen-cao/) if you'd like to connect!

---

# Experience

{% if site.work_experience %}
<div class="archive--card-grid">
  {% for post in site.work_experience reversed %}
    {% include archive-single-card.html post=post %}
  {% endfor %}
</div>
{% endif %}

---

# Publications

{% if site.publications %}
<div class="archive--card-grid">
  {% for post in site.publications reversed %}
    {% include archive-single-card.html post=post %}
  {% endfor %}
</div>
{% endif %}

---

# Projects

{% if site.portfolio %}
<div class="archive--card-grid">
  {% for post in site.portfolio reversed %}
    {% include archive-single-card.html post=post %}
  {% endfor %}
</div>
{% endif %}

---

# Achievements

{% if site.achievements %}
<div class="archive--card-grid">
  {% for post in site.achievements reversed %}
    {% include archive-single-card.html post=post %}
  {% endfor %}
</div>
{% endif %}

---

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/).