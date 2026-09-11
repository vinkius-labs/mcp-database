# CORDIS EU Research Funding MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cordis-eu-research-funding)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Official EU research & innovation funding database: search Horizon Europe and H2020 projects, exploitable results and news, full project factsheets with EU contribution amounts, coordinators and dates — zero auth.

## Description
**CORDIS** — the European Commission's official database of EU-funded research and innovation — as a single MCP server.

### What you can do
- **Search funded projects** across Horizon Europe, Horizon 2020, ERC and earlier programmes, filtered to project entries with acronyms and grant agreement IDs
- **Full project factsheets** — EU contribution, total cost, signature date, start/end dates, funding programme and coordinator institution, straight from the official page
- **Scout exploitable results** — technologies, prototypes and outcomes from EU projects available for transfer or commercialisation
- **News and briefs** — the Commission's own editorial coverage of funded research, in multiple languages
- **Programme filtering** — slice by Horizon Europe pillar or cluster (HORIZON.1–4, e.g. HORIZON.2.4 Digital/Industry/Space, HORIZON.3 = EIC), by language, or free-form
- **Programme code reference** — decode the pillar/cluster codes attached to every result

### Why CORDIS
CORDIS is the authoritative record of who received EU R&I money, for what, and with what outcomes. For startups it is competitive intelligence (who is funded in your space, from which institution, how much) and a partner-sourcing tool (find coordinators with a track record in your domain). For researchers and journalists it is the official archive. Every tool here runs keyless against the public CORDIS search API and fact-sheet pages.

### Typical workflows
- Benchmark EU funding levels in a topic area before applying
- Find a coordinator or partner institution with a proven track record
- Track exploitable technologies in your domain for scouting or M&A
- Follow the Commission's own reporting on a policy area


## Available Tools (8)
- **get_project_factsheet**: 3030/101178523). Returns: title, DOI, EC signature date, start/end dates, funding programme, total cost, EU contribution and coordinator with its funding. Use it to benchmark funding levels for a topic, find the coordinator institution, or check whether a project is still running.

Full official factsheet for one EU-funded project: budget (EU contribution), dates, programme, coordinator and link
- **search_all_content**: Each row carries contentType ("article", "result", "project", ...) and kind (news / brief / projectDescription / exploitableResult ...) so you can see what exists for a topic before drilling down with search_projects, search_results or search_news_articles. Query is MANDATORY. Great first tool for open-ended questions like "what is the EU funding in solid state batteries?".

Cross-content search over ALL CORDIS content types: projects, results, news articles, briefs and more
- **search_results**: Each row links to the origin project (projectId). Use for technology scouting: finding EU-funded innovations available in a domain, tracking what competitors of a technology exist, or sourcing partners with proven results. Query is MANDATORY.

Search exploitable R&I results published on CORDIS — technologies, prototypes and outcomes ready for transfer or commercialisation
- **search_news_articles**: This is the editorial coverage of EU-funded research — good for trends, success stories, policy signals and project summaries in readable form. Content arrives in multiple EU languages; pass language="en" to keep only English rows, or use search_content_by_language for other languages. Query is MANDATORY.

Search CORDIS news articles and project briefs — how the EU reports on funded research
- **find_projects_by_programme**: Programme codes look like HORIZON.1 (Excellent Science), HORIZON.2 (Global Challenges & Industrial Competitiveness — clusters .1 Health to .6 Space...), HORIZON.3 (Innovative Europe / EIC), H2020, ERC. Pass a full code ("HORIZON.2.2"), a pillar ("HORIZON.3"), a family ("H2020") or any substring — matching is case-insensitive and prefix-based. Combine with a topical query (q is MANDATORY). See get_programme_reference for the full code tree.

Find EU-funded content under a specific Horizon Europe pillar/cluster or programme (e.g. HORIZON.2.2, H2020, ERC)
- **search_content_by_language**: CORDIS publishes project descriptions in many EU languages and the raw index interleaves them — this tool makes results readable when a single language is wanted (usually "en"). Query is MANDATORY.

Search CORDIS keeping only content in a specific language (en, de, es, fr, it, pl, ...)
- **get_programme_reference**: 1 Excellent Science, HORIZON.2 Global Challenges with clusters .1 Health to .6 Space, HORIZON.3 Innovative Europe incl. the European Innovation Council), the European Research Council (ERC), Horizon 2020 (H2020) and Euratom. Use it to interpret codes returned by search tools or to pick a filter for find_projects_by_programme.

Reference: Horizon Europe / H2020 programme code tree used in CORDIS rows (pillars, clusters, EIC, ERC)
- **search_projects**: Use projectId with get_project_factsheet for budget, dates and coordinator. Query is MANDATORY and full-text: combine topic + domain keywords, e.g. "carbon capture steel", "AI healthcare diagnostics", "quantum computing Portugal". Results come in multiple EU languages (see search_content_by_language to force English). This search does NOT list open funding calls — use it to study who was funded, on what topics, for how much.

Search EU-funded research & innovation projects (Horizon Europe, H2020, ERC and earlier programmes) in the official CORDIS database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CORDIS EU Research Funding** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What EU funding has gone into solid state batteries? Find projects and how much the EU contributed."

**🤖 AI Agent:**
> 🔬 **EU funding in solid state batteries**

Key CORDIS projects found:
- **SOLIDIFY** (H2020) — solid-state lithium batteries for EVs; EU contribution ≈ €6.7M
- **IntelLiGent** — next-gen solid-state cells; EU contribution ≈ €4.9M

Let me pull the full factsheets (budgets, dates, coordinators) for the top matches — which one interests you most? I can also filter to a specific pillar (e.g. HORIZON.2.5 Climate/Energy) or look for exploitable results.

---

**👤 You:**
> "Which institutions coordinate Horizon Europe projects on AI for healthcare? I'm looking for a partner for my startup."

**🤖 AI Agent:**
> 🤝 **Potential coordinators — AI for healthcare (Horizon Europe)**

From CORDIS project search + factsheets:
- **KTH Royal Institute of Technology** (SE) — coordinator of 2 HE projects in AI diagnostics
- **University of Milano-Bicocca** (IT) — leads an AI clinical-decision cluster under HORIZON.2.1

Each has a proven track record in your exact domain. I can pull each project's budget and consortium size, then list exploitable results from their completed work.


## ❓ FAQ

**Q: Does this MCP list open funding calls I can apply to?**
No — CORDIS records funded projects and their outcomes, not open calls. Open calls live on the EU Funding & Tenders Portal. Use this MCP to study who was funded in your domain (topics, budgets, coordinators) and to source partners; then check the Funding Portal for live calls.

**Q: Do I need an API key, and why do results come in several languages?**
No key needed — CORDIS is fully public. CORDIS publishes content in many EU languages and the search index interleaves them; use search_content_by_language (e.g. language="en") or the language parameter on search_news_articles to keep a single language.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cordis-eu-research-funding](https://vinkius.com/en/ai-agent-connect/cordis-eu-research-funding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CORDIS EU Research Funding** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cordis-eu-research-funding` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CORDIS EU Research Funding** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cordis-eu-research-funding": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
