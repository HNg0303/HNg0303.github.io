---
permalink: /
title: "Quang-Binh Nguyen"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

I am a Research Resident at Qualcomm AI Research, advised by Dr. Khoi Nguyen. I obtained my Bachelor's Degree in Computer Science - Honors Program at University of Science, VNU-HCM, under the supervision of Prof. Minh-Triet Tran and Dr. Trung-Nghia Le.

My research focuses on controllable image generation, particularly image personalization (diffusion and autoregressive models). Recently, I have been working on test-time alignment for generative models.

Feel free to reach out via [email](mailto:chnguyen032005@gmail.com) or [LinkedIn](https://www.linkedin.com/in/hoang-nguyen-cao/) if you'd like to connect!

---

## Featured Sections

<div class="homepage-sections">

  <!-- About Me Section -->
  <section class="section-preview" id="about-section">
    <h2 class="section-title">
      <a href="{{ base_path }}/about-me/">About Me</a>
    </h2>
    <div class="section-content">
      <p>Learn more about my background, education, and research interests. I'm passionate about controllable image generation and making AI more accessible.</p>
      <a href="{{ base_path }}/about-me/" class="btn btn--primary">View Full Bio</a>
    </div>
  </section>

  <!-- Work Experience Section -->
  {% if site.work_experience %}
  <section class="section-preview" id="experience-section">
    <h2 class="section-title">
      <a href="{{ base_path }}/work-experience/">Work Experience</a>
    </h2>
    <div class="archive--card-grid">
      {% for post in site.work_experience reversed | limit: 3 %}
        {% include archive-single.html type="card" %}
      {% endfor %}
    </div>
    <a href="{{ base_path }}/work-experience/" class="btn btn--primary">View All Experience</a>
  </section>
  {% endif %}

  <!-- Publications Section -->
  {% if site.publications %}
  <section class="section-preview" id="publications-section">
    <h2 class="section-title">
      <a href="{{ base_path }}/publications/">Publications</a>
    </h2>
    <div class="archive--card-grid">
      {% for post in site.publications reversed | limit: 3 %}
        {% include archive-single.html type="card" %}
      {% endfor %}
    </div>
    <a href="{{ base_path }}/publications/" class="btn btn--primary">View All Publications</a>
  </section>
  {% endif %}

  <!-- Projects Section -->
  {% if site.portfolio %}
  <section class="section-preview" id="projects-section">
    <h2 class="section-title">
      <a href="{{ base_path }}/portfolio/">Projects</a>
    </h2>
    <div class="archive--card-grid">
      {% for post in site.portfolio reversed | limit: 3 %}
        {% include archive-single.html type="card" %}
      {% endfor %}
    </div>
    <a href="{{ base_path }}/portfolio/" class="btn btn--primary">View All Projects</a>
  </section>
  {% endif %}

  <!-- Achievements Section -->
  {% if site.achievements %}
  <section class="section-preview" id="achievements-section">
    <h2 class="section-title">
      <a href="{{ base_path }}/achievements/">Achievements</a>
    </h2>
    <div class="archive--card-grid">
      {% for post in site.achievements reversed | limit: 3 %}
        {% include archive-single.html type="card" %}
      {% endfor %}
    </div>
    <a href="{{ base_path }}/achievements/" class="btn btn--primary">View All Achievements</a>
  </section>
  {% endif %}

</div>

<style>
  .homepage-sections {
    margin: 2rem 0;
  }

  .section-preview {
    margin-bottom: 3rem;
    padding: 0;
  }

  .section-title {
    font-size: 1.75rem;
    margin-bottom: 1.5rem;
    padding-bottom: 1rem;
    border-bottom: 2px solid var(--global-border-color);
  }

  .section-title a {
    text-decoration: none;
    color: inherit;
  }

  .section-title a:hover {
    color: var(--global-text-color-light);
  }

  .section-content {
    margin-bottom: 1.5rem;
    padding: 1.5rem;
    background: var(--global-background-color-secondary, rgba(0, 0, 0, 0.02));
    border-radius: 6px;
  }

  .btn {
    display: inline-block;
    padding: 0.75rem 1.5rem;
    margin-top: 1rem;
    background-color: var(--global-text-color);
    color: var(--global-background-color);
    text-decoration: none;
    border-radius: 4px;
    transition: all 0.3s ease;
  }

  .btn:hover {
    background-color: var(--global-text-color-light);
    text-decoration: none;
  }

  .btn--primary {
    background-color: var(--global-text-color);
    color: var(--global-background-color);
  }

  .btn--primary:hover {
    background-color: var(--global-text-color-light);
  }

  .archive--card-grid {
    margin-bottom: 1.5rem;
  }
</style>
 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
