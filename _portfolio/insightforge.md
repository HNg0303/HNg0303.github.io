---
title: "InsightForge — Agentic Assistant for Content Creators"
collection: portfolio
permalink: /portfolio/insightforge/
date: 2026-03-01
status: "Active"
excerpt: "A sophisticated multi-agent system using Stateful LangGraph and MCP servers to automate trend discovery, script generation, and cross-platform publishing for content creators."

codeurl: "https://github.com/HNg0303/InsightForge"
tags:
  - LangGraph
  - MCP
  - A2A Protocol
  - Multi-Agent
  - LLM
  - Python
---

## Overview

**InsightForge** is an agentic assistant built for content creators. It automates the full content production pipeline — from discovering trending topics to generating scripts and publishing across platforms — reducing creator workflow time by **40%**.

Built during **GDGoC Hackathon 2026** where the team placed **Top 2 / 300** teams (Finalist).

## Architecture

The system uses a **Stateful LangGraph** graph as the orchestration backbone, with specialized sub-agents communicating via the **A2A (Agent2Agent) Protocol**:

- **Trend Discovery Agent**: Crawls and aggregates trending topics across platforms using MCP-connected tools.
- **Script Generation Agent**: Produces structured content outlines and full scripts grounded in trending data.
- **Publishing Agent**: Handles cross-platform formatting and scheduling.

### Key Design Decisions

- **MCP (Model Context Protocol) Servers**: Standardized tool interfaces for web crawling, search, and content APIs.
- **A2A Protocol**: Ensures type-safe JSON payloads between agents, enabling seamless state and data exchange.
- **Structured Output Validation**: LLM backbone outputs are validated against Pydantic schemas before being consumed downstream.
- **Multi-LLM Support**: Pluggable backbone supporting Gemini, GPT-4o, and Claude.

## Tech Stack

| Layer | Stack |
|---|---|
| Orchestration | LangGraph (Stateful) |
| Agent Communication | A2A Protocol |
| Tool Access | MCP Servers |
| LLM Backends | Gemini / GPT-4o / Claude |
| Language | Python |

## System Architecture

![InsightForge Architecture Diagram](/images/projects/InsightForge_Architecture.png)

The system orchestrates three specialized agents:
- **Trend Analysis Agent**: Real-time trend discovery across Google Trends, TikTok, and Threads
- **Content Architect Agent**: Script generation with structured outlines and multimedia cues
- **Posting Agent**: Cross-platform formatting and automated scheduling

## Workflow

![Multi-Agent Workflow](/images/projects/InsightForge_Workflow.png)

User queries are routed through a **Stateful LangGraph** orchestrator that:
1. Analyzes trending topics
2. Generates structured content
3. Requests human approval before publishing
4. Executes publishing with feedback loops for continuous refinement

## Recognition

![GDGoC Hackathon Certificate](/images/projects/InsightForge_Certificate.png)

## Impact

- 🏆 **GDGoC Hackathon Vietnam 2026** — Finalist, Top 2 / 300 (AI Content Architecture track)
- Reduced content creator research-to-script workflow time by ~40%
