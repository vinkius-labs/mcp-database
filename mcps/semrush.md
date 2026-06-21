# Semrush MCP Server

Grant your AI agent access to Semrush's massive SEO database to analyze competitor backlink profiles, track domain ranks, and research profitable keywords contextually.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/semrush)

## Overview
**Category:** growth-engine
**Tools Count:** 8

## Description
Equip your conversational workflow with the raw data power of **Semrush**, the industry standard for Digital Marketing visibility. Through this server, your AI can pull immense amounts of SERP forensics directly into the context window. Stop switching tabs to look up keyword difficulty—just command your agent to fetch it seamlessly.

### What you can do

- **Deep Domain Forensics (Competitors)** — Query `domain_overview` or `domain_vs_domain` to tell your agent to digest the exact organic search volume differences between you and a rival
- **Keyword Strategy Building** — Hand a seed topic to the LLM and invoke `related_keywords`. The AI will compile comprehensive editorial briefs loaded with actual search volumes and CPCs
- **Backlink Auditing** — Track the inbound link profile (`get_backlinks`) of external domains to gauge authority natively within chat sessions
- **Technical SEO Interrogation** — Quickly bring your technical `site_audit` score to the AI, asking it to explain what the flagged errors mean and draft instructions to fix missing metadata

### How it works

1. Enable the Semrush MCP Server on your local environment
2. Authorize using your top-tier Semrush Business API Key
3. Interface with advanced LLMs (like Claude) using direct conversational requests to interrogate organic traffic algorithms

### Who is this for?

- **SEO Strategists** — skip the spreadsheet formatting; ask the AI to download top organic keywords and summarize the competitive landscape instantly
- **Content Marketers** — have your IDE write an article and dynamically insert LSI (Latent Semantic Indexing) keywords pulled dynamically from `keyword_overview`
- **Digital Analysts** — command the bot to fetch `traffic_analytics` on five different disruptive startups to assess bounce rates side-by-side


## Available Tools
- **domain_overview**: Specify the database (e.g., "us", "uk") if targeting a specific region.

Get domain SEO overview: rank, organic traffic, paid traffic
- **organic_keywords**: Useful for competitor analysis or performance tracking.

Get domain organic keyword positions
- **keyword_overview**: Get keyword metrics: volume, CPC, competition, SERP features
- **related_keywords**: Ideal for content planning and SEO expansion.

Get related keywords with volume and difficulty
- **get_backlinks**: Get backlink overview for a domain
- **domain_vs_domain**: Compare two domains SEO side by side
- **traffic_analytics**: Get traffic analytics: visits, bounce rate, pages/visit
- **site_audit**: Requires a valid Semgrep project ID.

Get site audit quality overview for a project


## Installation & Usage

To install and use the **Semrush** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semrush](https://vinkius.com/mcp/semrush)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
