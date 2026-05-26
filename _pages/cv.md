---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Outfit:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>
  :root {
    --accent: #6366f1;
    --accent-soft: rgba(99, 102, 241, 0.08);
    --border: rgba(120, 120, 120, 0.15);
    --text-soft: #6b7280;
  }

  .cv-page {
    font-family: 'Outfit', sans-serif;
    line-height: 1.75;
  }

  .cv-hero {
    margin: 1rem 0 2rem 0;
    padding: 1.5rem 1.75rem;
    border-radius: 18px;
    background: linear-gradient(
      135deg,
      rgba(99, 102, 241, 0.08),
      rgba(168, 85, 247, 0.05)
    );
    border: 1px solid var(--border);
  }

  .cv-hero h1 {
    margin: 0;
    font-size: 2rem;
    font-weight: 700;
  }

  .cv-hero p {
    margin-top: 0.8rem;
    color: var(--text-soft);
    font-size: 1rem;
  }

  .cv-section {
    margin-top: 2.5rem;
  }

  .cv-section-title {
    display: flex;
    align-items: center;
    gap: 10px;
    margin-bottom: 1.2rem;
    font-size: 1.35rem;
    font-weight: 700;
    letter-spacing: -0.02em;
  }

  .cv-section-title::after {
    content: "";
    flex: 1;
    height: 1px;
    background: linear-gradient(to right, var(--accent), transparent);
  }

  .cv-card {
    border: 1px solid var(--border);
    border-radius: 16px;
    padding: 1.2rem 1.3rem;
    margin-bottom: 1rem;
    transition: all 0.2s ease;
    background: rgba(255,255,255,0.02);
  }

  .cv-card:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 20px rgba(0,0,0,0.05);
  }

  .cv-card-header {
    display: flex;
    justify-content: space-between;
    gap: 1rem;
    flex-wrap: wrap;
    margin-bottom: 0.5rem;
  }

  .cv-role {
    font-size: 1.05rem;
    font-weight: 600;
  }

  .cv-date {
    font-size: 0.92rem;
    color: var(--text-soft);
    font-family: 'DM Mono', monospace;
  }

  .cv-org {
    color: var(--accent);
    font-weight: 500;
    margin-bottom: 0.7rem;
  }

  .cv-card ul {
    padding-left: 1.2rem;
    margin: 0.4rem 0 0 0;
  }

  .cv-card li {
    margin-bottom: 0.55rem;
  }

  .cv-highlight {
    font-weight: 600;
    color: var(--accent);
  }

  .cv-skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 16px;
    margin-top: 1rem;
    margin-bottom: 2rem;
  }

  .cv-skill-card {
    background: var(--background-color, #ffffff);
    border: 0.5px solid rgba(128, 128, 128, 0.2);
    border-radius: 14px;
    padding: 16px 18px;
    position: relative;
    overflow: hidden;
    transition: transform 0.2s ease, border-color 0.2s ease, box-shadow 0.2s ease;
  }

  .cv-skill-card:hover {
    transform: translateY(-3px);
    border-color: rgba(128, 128, 128, 0.4);
    box-shadow: 0 4px 12px rgba(0, 0, 0, 0.05);
  }

  .cv-skill-card::before {
    content: '';
    position: absolute;
    top: 0; left: 0; right: 0;
    height: 3px;
    background: var(--card-accent, #6366f1);
    opacity: 0.85;
  }

  .c-lang { --card-accent: #3b82f6; }
  .c-dl { --card-accent: #8b5cf6; }
  .c-agent { --card-accent: #6366f1; }
  .c-back { --card-accent: #10b981; }
  .c-front { --card-accent: #ec4899; }
  .c-other { --card-accent: #f59e0b; }

  .cv-skill-header {
    display: flex;
    align-items: center;
    gap: 10px;
    font-weight: 600;
    font-size: 15px;
    margin-bottom: 14px;
  }

  .cv-skill-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 28px;
    height: 28px;
    border-radius: 8px;
    background: rgba(128, 128, 128, 0.08);
    font-size: 14px;
  }

  .cv-skill-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 6px;
  }

  .cv-skill-tag {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    padding: 4px 10px;
    border-radius: 6px;
    background: rgba(128, 128, 128, 0.05);
    border: 0.5px solid rgba(128, 128, 128, 0.18);
    transition: all 0.2s ease;
  }

  .cv-skill-tag:hover {
    background: rgba(128, 128, 128, 0.12);
  }

  @media (prefers-color-scheme: dark) {
    .cv-skill-card {
      background: #171717;
    }

    .cv-card {
      background: rgba(255,255,255,0.02);
    }

    .cv-skill-tag {
      background: rgba(255, 255, 255, 0.04);
      border-color: rgba(255, 255, 255, 0.1);
    }
  }
</style>

<div class="cv-page">

<div class="cv-hero">
  <h1>AI Engineer / Research-Oriented CS Student</h1>
  <p>
    Junior (3rd Year) Computer Science student focused on AI systems, agentic workflows,
    RAG pipelines, and Generative AI. Passionate about building
    production-ready intelligent systems and conducting applied AI research.
  </p>
</div>

<div class="cv-section">
  <div class="cv-section-title">🎓 Education</div>

  <div class="cv-card">
    <div class="cv-card-header">
      <div class="cv-role">
        B.S. in Computer Science (APCS)
      </div>
      <div class="cv-date">2023 – 2027 (Expected)</div>
    </div>

    <div class="cv-org">
      Ho Chi Minh University of Science, VNUHCM
    </div>

    <ul>
      <li><span class="cv-highlight">GPA:</span> 3.83 / 4.0</li>
      <li>
        Relevant Coursework:
        Natural Language Processing, Information Retrieval,
        Artificial Intelligence, Software Engineering
      </li>
    </ul>
  </div>
</div>

<div class="cv-section">
  <div class="cv-section-title">💼 Experience</div>

  <div class="cv-card">
    <div class="cv-card-header">
      <div class="cv-role">
        Undergraduate Research Assistant
      </div>
      <div class="cv-date">Oct 2025 – Present</div>
    </div>

    <div class="cv-org">
      Ho Chi Minh University of Science, VNUHCM
    </div>

    <ul>
      <li>
        Research in Vision-Language Models (VLMs),
        cross-modal retrieval, and Generative AI under PhD supervision.
      </li>

      <li>
        Co-authored first-author paper accepted at
        ACM ICMR 2026 (Amsterdam).
      </li>

      <li>
        Executed the full research pipeline including
        dataset curation, model fine-tuning,
        benchmark design, and manuscript review.
      </li>
    </ul>
  </div>
</div>

<div class="cv-section">
  <div class="cv-section-title">🚀 Projects</div>

  <div class="cv-card">
    <div class="cv-card-header">
      <div class="cv-role">
        INSIGHTFORGE — Agentic Assistant for Content Creators
      </div>
      <div class="cv-date">Mar 2026 – Present</div>
    </div>

    <ul>
      <li>
        Designed a multi-agent system using Stateful LangGraph and MCP servers
        to automate trend discovery, script generation,
        and cross-platform publishing.
      </li>

      <li>
        Reduced creator workflow time by
        <span class="cv-highlight">40%</span>.
      </li>

      <li>
        Standardized inter-agent communication using
        A2A Protocol for seamless state and data exchange.
      </li>

      <li>
        Integrated Gemini, GPT-4o, and Claude with structured output validation
        for type-safe downstream workflows.
      </li>
    </ul>
  </div>

  <div class="cv-card">
    <div class="cv-card-header">
      <div class="cv-role">
        RAGNEWS — Agentic LLM-Powered News Platform
      </div>
      <div class="cv-date">Jan 2026 – Mar 2026</div>
    </div>

    <ul>
      <li>
        Built an asynchronous agentic RAG pipeline using
        FastAPI and LangChain with autonomous routing tools.
      </li>

      <li>
        Implemented a two-stage retrieval architecture using
        Milvus and BGE-Reranker for lower latency retrieval.
      </li>

      <li>
        Fine-tuned Qwen2.5-1.5B via LoRA and Unsloth
        for domain-specific summarization tasks.
      </li>

      <li>
        Reduced training memory footprint by
        <span class="cv-highlight">60%</span>.
      </li>

      <li>
        Deployed inference using vLLM with PostgreSQL persistence
        and a Streamlit interface for interactive sessions.
      </li>
    </ul>
  </div>
</div>

<div class="cv-section">
  <div class="cv-section-title">🏆 Achievements</div>

  <div class="cv-card">
    <ul>
      <li>
        Finalist — Top 2/300 GDGoC Hackathon Vietnam 2026
        (AI Content Architecture), Hanoi
      </li>

      <li>
        Finalist — Top 24/200 Techcombank HackCX-Together 2025
        (AI Banking Assistant), Hanoi
      </li>
    </ul>
  </div>
</div>

<div class="cv-section">
  <div class="cv-section-title">📚 Publications</div>

  <ul>
    {% for post in site.publications reversed %}
      {% include archive-single-cv.html %}
    {% endfor %}
  </ul>
</div>

<div class="cv-section">
  <div class="cv-section-title">🛠 Skills</div>

  <div class="cv-skills-grid">

    <div class="cv-skill-card c-lang">
      <div class="cv-skill-header">
        <div class="cv-skill-icon">💻</div>
        Languages
      </div>

      <div class="cv-skill-tags">
        <span class="cv-skill-tag">Python</span>
        <span class="cv-skill-tag">C++</span>
        <span class="cv-skill-tag">JavaScript</span>
      </div>
    </div>

    <div class="cv-skill-card c-dl">
      <div class="cv-skill-header">
        <div class="cv-skill-icon">🧠</div>
        Deep Learning
      </div>

      <div class="cv-skill-tags">
        <span class="cv-skill-tag">PyTorch</span>
        <span class="cv-skill-tag">Transformers</span>
        <span class="cv-skill-tag">LoRA / PEFT</span>
        <span class="cv-skill-tag">Unsloth</span>
        <span class="cv-skill-tag">vLLM</span>
        <span class="cv-skill-tag">Scikit-Learn</span>
      </div>
    </div>

    <div class="cv-skill-card c-agent">
      <div class="cv-skill-header">
        <div class="cv-skill-icon">🤖</div>
        Agentic Systems
      </div>

      <div class="cv-skill-tags">
        <span class="cv-skill-tag">LangChain</span>
        <span class="cv-skill-tag">LangGraph</span>
        <span class="cv-skill-tag">MCP</span>
        <span class="cv-skill-tag">A2A Protocol</span>
      </div>
    </div>

    <div class="cv-skill-card c-back">
      <div class="cv-skill-header">
        <div class="cv-skill-icon">⚙️</div>
        Backend & DB
      </div>

      <div class="cv-skill-tags">
        <span class="cv-skill-tag">FastAPI</span>
        <span class="cv-skill-tag">PostgreSQL</span>
        <span class="cv-skill-tag">Docker</span>
        <span class="cv-skill-tag">Milvus</span>
        <span class="cv-skill-tag">Qdrant</span>
        <span class="cv-skill-tag">FAISS</span>
      </div>
    </div>

    <div class="cv-skill-card c-front">
      <div class="cv-skill-header">
        <div class="cv-skill-icon">🎨</div>
        Frontend
      </div>

      <div class="cv-skill-tags">
        <span class="cv-skill-tag">ReactJS</span>
        <span class="cv-skill-tag">NextJS</span>
        <span class="cv-skill-tag">Streamlit</span>
      </div>
    </div>

    <div class="cv-skill-card c-other">
      <div class="cv-skill-header">
        <div class="cv-skill-icon">🌟</div>
        Others
      </div>

      <div class="cv-skill-tags">
        <span class="cv-skill-tag">IELTS 7.5</span>
        <span class="cv-skill-tag">Teamwork</span>
        <span class="cv-skill-tag">Presentation</span>
      </div>
    </div>

  </div>
</div>

</div>