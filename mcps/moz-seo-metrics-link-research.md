# Moz (SEO Metrics & Link Research) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moz-seo-metrics-link-research)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moz-seo-metrics-link-research-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moz-seo-metrics-link-research-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage SEO metrics via Moz — audit Domain Authority (DA), analyze backlinks, and track site rankings.

## Description
Connect your **Moz API** account to any AI agent and take full control of your search engine optimization, link research, and competitive intelligence through natural conversation.

### What you can do

- **Authority Orchestration** — Retrieve precise Domain Authority (DA) and Page Authority (PA) scores for any URL or root domain to understand ranking potential directly from your agent
- **Backlink Audit** — List incoming and outgoing links for specific domains, extracting source URLs, anchor texts, and equity boundaries to identify high-value linking opportunities
- **Competitive Intelligence** — Compare multiple target domains simultaneously to retrieve side-by-side metrics including spam scores and literal link counts securely
- **Anchor Text Analysis** — Extract the literal distribution of anchor text across your backlink profile to understand semantic density and keyword relevance natively
- **Top Pages Discovery** — Query the most internally and externally linked pages within a domain, sorted by Page Authority, to identify high-equity content assets
- **Global Web Rankings** — Access globally tracked lists of top root domains and pages based on Moz's massive link index to benchmark against industry leaders
- **Usage Monitoring** — Track your API row consumption and remaining quotas in real-time to manage your research budget and avoid automated service halts

### How it works

1. Subscribe to this server
2. Enter your Moz API V3 Token
3. Start optimizing your search presence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO Specialists** — analyze domain authority and audit link equity through natural conversation without manual keyword research tools
- **Digital Marketers** — track backlink profiles and monitor competitive site metrics directly from your workspace
- **Content Strategists** — identify top-performing pages and analyze anchor text distributions efficiently to guide content production


## Available Tools
- **get_url_metrics**: 0 metrics defining explicitly domain rankings and literal link equity boundaries.

Get Moz API V3 Domain Authority (DA) Page Authority (PA) spam scoring and mapped exact link counts
- **get_incoming_links**: Get explicit incoming backlinks hitting a specific domain mapping Moz API link index
- **get_outgoing_links**: Get explicit outgoing external links originating from a target mapping outbound anchor texts
- **get_top_links**: Get explicitly top-ranked backlinks mapped directly onto a domain sorted primarily by Domain Authority
- **get_anchor_text**: Analyze literal anchor text distribution matching backlinks that point to an explicit domain
- **get_linking_domains**: Get summarized root linking domains hitting specific bounds
- **get_top_pages**: Query top-performing literal pages existing inside an explicit domain sorted by highest internal linking/PA
- **global_top_pages**: Extract static global Top Pages across entire web indexed by Moz metric systems
- **global_top_domains**: Extract static global Top root Domains evaluating worldwide highest DA metrics
- **get_usage**: Check running quota tracking for current Moz API rows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moz (SEO Metrics & Link Research)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get Moz metrics for 'moz.com' and 'ahrefs.com'"

**🤖 AI Agent:**
> Retrieving metrics… For 'moz.com', the DA is 91 and the Spam Score is 1%. For 'ahrefs.com', the DA is 90 with a 2% Spam Score. Both domains show very high authority. Would you like me to compare their top incoming backlinks?

---

**👤 You:**
> "List the top 5 incoming links for 'stripe.com' sorted by authority"

**🤖 AI Agent:**
> Retrieving backlinks… I've identified the top sources: 1) apple.com (PA: 95), 2) nytimes.com (PA: 94), 3) github.com (PA: 92), 4) wired.com (PA: 90), and 5) techcrunch.com. These high-equity links contribute significantly to Stripe's DA. Would you like to see the anchor text for these links?

---

**👤 You:**
> "Show me the anchor text distribution for 'vercel.com'"

**🤖 AI Agent:**
> Analyzing anchor text… For 'vercel.com', the distribution is: 'vercel' (45%), 'next.js' (22%), 'deploy' (12%), 'https://vercel.com' (8%), and 'frontend cloud' (5%). The profile looks very natural with strong brand association. Would you like me to identify which domains use the 'frontend cloud' anchor?


## Installation & Usage

To install and use the **Moz (SEO Metrics & Link Research)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moz-seo-metrics-link-research](https://vinkius.com/mcp/moz-seo-metrics-link-research)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
