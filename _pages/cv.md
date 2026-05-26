---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Summary
======
* [cite_start]I am currently a Junior (3rd year) Computer Science student with a strong focus in AI and hands-on experience building production RAG pipelines, multi-agent systems, and fine-tuned LLMs. [cite: 4]
* I have a strong background in agentic frameworks, retrieval systems, and efficient LLM model adaptation. [cite_start]I am seeking an Intern/Fresher AI Engineer role. [cite: 5]

Education
======
* [cite_start]B.S. in Computer Science (APCS), Ho Chi Minh University of Science, VNUHCM, 2023 - 2027 (Expected) [cite: 7, 8, 9]
  * [cite_start]Cumulative GPA: 3.83/4.0 [cite: 8]
  * [cite_start]Relevant Coursework: Natural Language Processing, Information Retrieval, Artificial Intelligence, Software Engineer. [cite: 10]

Work experience
======
* [cite_start]Oct 2025 - Present: Undergraduate Research Assistant [cite: 13, 14]
  * [cite_start]Ho Chi Minh University of Science, VNUHCM [cite: 12]
  * [cite_start]Research in Vision-Language Models (VLMs), cross-modal retrieval, and Generative AI under PhD supervision. [cite: 15]
  * [cite_start]Co-authored first-author paper accepted at ACM ICMR 2026 (Amsterdam) B-Rank/Top-tier venue. [cite: 16]
  * [cite_start]Executed full research pipeline: dataset curation, model fine-tuning, benchmark design, and manuscript review. [cite: 17]

Projects
======
* [cite_start]INSIGHTFORGE - Agentic Assistant for Content Creators (March 2026 - Present) [cite: 19, 20]
  * [cite_start]Designed a sophisticated multi-agent system using Stateful LangGraph and MCP (Model Context Protocol) servers to automate trend discovery, script generation, and cross-platform publishing - reduced creator workflow time by 40%. [cite: 20]
  * [cite_start]Standardized communication between agents using A2A (Agent2Agent) Protocol for seamless state and data exchange. [cite: 21]
  * [cite_start]Integrated LLM backbone (Gemini / GPT-4o / Claude) with structured output validation, ensuring downstream agents receive type-safe JSON payloads. [cite: 22]

* [cite_start]RAGNEWS - Agentic LLM-Powered News Platform (January 2026 - March 2026) [cite: 23, 24]
  * [cite_start]Pipeline & Agent Engineering: Designed an asynchronous, agentic RAG pipeline using FastAPI and LangChain, integrating database-aware tools to autonomously route user queries and manage concurrent data ingestion. [cite: 25]
  * [cite_start]Advanced Retrieval Architecture: Implemented a two-stage retrieval system, minimizing search latency by decoupling coarse-grained vector retrieval (Milvus) from compute-intensive cross-encoder re-ranking (BGE-Reranker). [cite: 26]
  * [cite_start]LLM Fine-Tuning & Analysis: Fine-tuned Qwen2.5-1.5B via LoRA and Unsloth for domain-specific summarization, and integrated a BERT-based sentiment classifier for financial news analysis, reducing training memory footprint by 60%. [cite: 27]
  * [cite_start]Production Serving & Persistence: Deployed the fine-tuned generative models using vLLM for high-throughput inference, a PostgreSQL database for short-term and long-term AI Conversation and a Streamlit UI for interactive sessions. [cite: 28]

Skills
======
* [cite_start]Languages: Python (primary), C++, JavaScript [cite: 37]
* [cite_start]Deep Learning Frameworks: PyTorch, Hugging Face Transformers, LoRA / PEFT, Unsloth, vLLM, Skicit-Learn [cite: 39]
* [cite_start]Agentic Frameworks: LangChain, LangGraph, MCP, A2A Protocol [cite: 40]
* [cite_start]Backend: FastAPI, PostgreSQL, Docker, Vector Database (Milvus, QDrant, FAISS) [cite: 41]
* [cite_start]Frontend: ReactJS, NextJS, Streamlit [cite: 42]
* [cite_start]Others: IELTS 7.5, Teamwork, Presentation [cite: 43]

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Achievements
======
* Finalist - Top 2/300 GDGoC Hackathon Vietnam 2026 (AI Content Architecture), Hanoi, April 2026 [cite: 34, 38]
* Finalist - Top 24/200 Techcombank HackCX-Together 2025 (AI Banking Assistant), Hanoi, June 2025 [cite: 34, 36, 38]

Skills
======

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=Outfit:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>
  .cv-skills-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 16px;
    margin-top: 1rem;
    margin-bottom: 2rem;
    font-family: 'Outfit', sans-serif;
  }
  .cv-skill-card {
    background: var(--background-color, #ffffff);
    border: 0.5px solid rgba(128, 128, 128, 0.2);
    border-radius: 12px;
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
    top: 0; left: 0; right: 0; height: 3px;
    background: var(--card-accent, #6366f1);
    opacity: 0.85;
  }
  /* Category specific accents */
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
    letter-spacing: 0.2px;
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
    color: inherit;
    transition: all 0.2s ease;
    cursor: default;
  }
  .cv-skill-tag:hover {
    background: rgba(128, 128, 128, 0.12);
    border-color: rgba(128, 128, 128, 0.3);
  }

  @media (prefers-color-scheme: dark) {
    .cv-skill-card {
      background: var(--background-color, #1a1a2e);
    }
    .cv-skill-tag {
      background: rgba(255, 255, 255, 0.04);
      border-color: rgba(255, 255, 255, 0.1);
    }
    .cv-skill-tag:hover {
      background: rgba(255, 255, 255, 0.1);
    }
  }
</style>

<div class="cv-skills-grid">
  
  <div class="cv-skill-card c-lang">
    <div class="cv-skill-header">
      <div class="cv-skill-icon">💻</div>
      Languages
    </div>
    <div class="cv-skill-tags">
      <span class="cv-skill-tag" style="background: rgba(59,130,246,0.1); border-color: rgba(59,130,246,0.3); color: #3b82f6;">Python (Primary)</span>
      <span class="cv-skill-tag">C++</span>
      <span class="cv-skill-tag">JavaScript</span>
    </div>
  </div>

  <div class="cv-skill-card c-dl">
    <div class="cv-skill-header">
      <div class="cv-skill-icon">🧠</div>
      Deep Learning Frameworks
    </div>
    <div class="cv-skill-tags">
      <span class="cv-skill-tag">PyTorch</span>
      <span class="cv-skill-tag">Hugging Face</span>
      <span class="cv-skill-tag">LoRA / PEFT</span>
      <span class="cv-skill-tag">Unsloth</span>
      <span class="cv-skill-tag">vLLM</span>
      <span class="cv-skill-tag">Scikit-Learn</span>
    </div>
  </div>

  <div class="cv-skill-card c-agent">
    <div class="cv-skill-header">
      <div class="cv-skill-icon">🤖</div>
      Agentic Frameworks
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
      Backend & Database
    </div>
    <div class="cv-skill-tags">
      <span class="cv-skill-tag">FastAPI</span>
      <span class="cv-skill-tag">PostgreSQL</span>
      <span class="cv-skill-tag">Docker</span>
      <span class="cv-skill-tag">Milvus</span>
      <span class="cv-skill-tag">QDrant</span>
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
      <span class="cv-skill-tag" style="background: rgba(245,158,11,0.1); border-color: rgba(245,158,11,0.3); color: #d97706;">IELTS 7.5</span>
      <span class="cv-skill-tag">Teamwork</span>
      <span class="cv-skill-tag">Presentation</span>
    </div>
  </div>

</div>