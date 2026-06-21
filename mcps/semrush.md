# Semrush MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/semrush)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Grant your AI agent access to Semrush's massive SEO database to analyze competitor backlink profiles, track domain ranks, and research profitable keywords contextually.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Semrush** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Pull the foundational organic ranking and paid traffic overview for the domain 'airbnb.com'. Target the US database."

**🤖 AI Agent:**
> Using the 'us' database configuration on `domain_overview`, I found that 'airbnb.com' commands a massive overarching Authority Score. Their organic search yields approximately 12.8M monthly hits relying on short-head housing terms, while their exact Paid Traffic scale denotes ~3.4M monthly clicks pushed primarily through Google Sponsored verticals.

---

**👤 You:**
> "Find 10 related keywords for the term 'buy mechanical keyboard' including their respective difficulties and search volumes."

**🤖 AI Agent:**
> I processed `related_keywords` targeting 'buy mechanical keyboard'. Let's focus on three prominent signals out of the 10 fetched: 1) 'best mechanical keyboard 2024' (Volume: 24K, KD: 78%). 2) 'buy cheap wired mechanical keyboard' (Volume: 8K, KD: 42%). 3) 'buy tactile mechanical keyboard red switches' (Volume: 3.5k, KD: 27%). The third option presents an excellent low-competition long-tail entry point.

---

**👤 You:**
> "Compare the overarching inbound domain performance between 'coca-cola.com' and 'pepsi.com'."

**🤖 AI Agent:**
> I executed `domain_vs_domain` between the corporate endpoints. Both share astronomically similar Authority Scores (~91). Coca-Cola leads marginally in total referring domains (approx. 240k unique backlinking entities), while Pepsi tracks slightly higher on brand-name aggregate search volume in the US. However, Coca-Cola is currently picking up 15% more non-brand long-tail queries overall.


## ❓ FAQ

**Q: Are there additional charges for querying Semrush from my agent?**
The Semrush API inherently consumes 'API Units' based on the weight of each request line (Keyword ranks, Domain analytics). You are completely bound to your established Semrush Business subscription rules. Vurb/MCP itself doesn't impose surcharges.

**Q: Can I filter SEO performance based on different global markets or languages?**
Yes. Most core functions such as `domain_overview` and `keyword_overview` optionally accept a targeted string code array for Regional Databases (such as 'uk', 'fr', 'de', 'es', or strictly 'us'). Just specify it organically in your LLM chatting window.

**Q: Can it check a website's technical health natively?**
Yes, through the specific `site_audit` directive. The AI agent will ingest the aggregated technical score corresponding directly to your preconfigured Semrush Project IDs, returning high-level data regarding crawled warnings and crawler fatal errors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/semrush](https://vinkius.com/mcp/semrush)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Semrush** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `semrush` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Semrush** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "semrush": {
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
