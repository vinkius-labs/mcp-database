# DeckMatch MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deckmatch)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/deckmatch-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/deckmatch-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Match startup pitch decks with investors using AI that analyzes fit, tracks outreach, and surfaces the right funding connections.

## Description
Connect your **DeckMatch** (now AlphaLens) account to any AI agent and take full control of your venture capital deal flow and startup analysis workflows through natural conversation.

### What you can do

- **Deck Orchestration** — Submit pitch deck URLs (PDF, PPTX, DocSend) programmatically to trigger automated data extraction and high-fidelity analysis
- **Investment Intelligence** — Programmatically generate professional investment memos and retrieve AI-driven triage results, including problem/solution and business models
- **Semantic Discovery** — Use the AlphaLens search engine to find startups matching specific strategic criteria and identify market signals directly through your agent
- **Portfolio Monitoring** — Access your complete directory of analyzed decks and monitor triage statuses to maintain perfectly coordinated deal flow pipelines
- **Operational Monitoring** — Check API health status, retrieve audit logs, and manage organization tags to maintain high-fidelity records of your investment activity

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your DeckMatch/AlphaLens dashboard settings
3. Start analyzing startup decks and searching your portfolio from Claude, Cursor, or any MCP client

No more manual data entry for every deck. Your AI acts as your dedicated investment associate and portfolio coordinator.

### Who is this for?

- **Venture Capitalists & VCs** — instantly retrieve triage summaries and check startup metrics using natural language commands
- **Investment Associates** — automate the generation of investment memos and track deal statuses without leaving your workspace
- **Accelerator Managers** — monitor incoming applications and search for relevant startups through simple AI queries


## Available Tools
- **tag_submission**: Label a submission
- **delete_submission**: Remove pitch deck
- **generate_investment_memo**: Create investment memo
- **get_api_status**: Get connectivity info
- **get_deck_analysis**: Get AI triage results
- **get_submission_audit**: Get audit trail
- **get_submission_details**: Get full submission info
- **list_enrichment_sources**: Get data sources
- **list_submissions**: List all analyzed decks
- **list_submission_tags**: List available tags
- **search_startups_semantically**: Find similar startups
- **submit_pitch_deck**: Submit a deck for AI analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeckMatch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this pitch deck: 'https://docsend.com/view/example-deck'."

**🤖 AI Agent:**
> Deck submission triggered! I've started the analysis for your DocSend URL. The job ID is 'sub_123'. I'll monitor the triage results and notify you as soon as the investment memo is ready.

---

**👤 You:**
> "Find startups similar to 'Stripe' focusing on 'climate tech payments'."

**🤖 AI Agent:**
> Searching portfolio... Using AlphaLens, I found 3 relevant startups: 'ClimatePay', 'CarbonSettlements' (Seed), and 'EcoFin'. Would you like the detailed triage summaries for these matches?

---

**👤 You:**
> "Generate an investment memo for submission 'sub_123'."

**🤖 AI Agent:**
> Memo generation complete! I've automatically crafted a professional investment memo for submission sub_123 based on the pitch deck analysis. You can now access the full document content.


## Installation & Usage

To install and use the **DeckMatch** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deckmatch](https://vinkius.com/mcp/deckmatch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
