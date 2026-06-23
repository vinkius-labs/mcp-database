# Raven Tools MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/raven-tools)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track SEO rankings, audit website health, and generate white-label marketing reports for your clients automatically.

## Description
Connect your **Raven Tools** account to any AI agent and take full control of your search engine optimization (SEO) orchestration and automated reporting through natural conversation.

### What you can do

- **Keyword Portfolio Orchestration** — List and manage your entire high-fidelity database of keyword rankings programmatically, retrieving detailed SERP position metadata
- **SEO Audit Intelligence Architecture** — Programmatically query and monitor website audit results to maintain a perfectly coordinated optimization pipeline
- **Backlink & Authority Monitoring** — Access your complete directory of high-fidelity backlinks and domain metrics to oversee your organizational visibility in real-time
- **Site Performance Monitoring** — Access real-time status updates for website health and track technical SEO metrics directly through your agent for instant reporting
- **Operational Monitoring** — Verify account-level API connectivity and monitor reporting volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Raven Tools dashboard (Settings > API)
3. Start orchestrating your SEO growth from Claude, Cursor, or any MCP client

No more manual exporting of keyword sheets or missing rank drops. Your AI acts as your dedicated SEO coordinator and reporting architect.

### Who is this for?

- **SEO Specialists** — instantly retrieve ranking summaries and monitor site health using natural language commands
- **Marketing Agencies** — verify individual project metadata and track client SEO progress without leaving your creative workspace
- **Developers** — integrate high-speed Raven Tools data into custom dashboards and reporting tools through simple AI queries


## Available Tools (12)
- **add_competitor**: Add a competitor
- **add_keyword**: Add a keyword
- **check_raventools_status**: Verify connectivity
- **get_links**: Get backlinks
- **get_project**: Get project info
- **get_rank_all**: Get all rankings
- **get_rank**: Get keyword rank
- **get_site_audit**: Get site audit
- **list_competitors**: List competitors
- **list_keywords**: List keywords
- **list_projects**: List projects/domains
- **remove_keyword**: Remove a keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Raven Tools** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects in my Raven Tools account and show the keyword summary for 'Project A'."

**🤖 AI Agent:**
> I've retrieved your projects. You currently have 10 active high-fidelity portfolios. For 'Project A' (ID: proj_123), I've identified 50 tracked keywords with an average SERP position of 5. Would you like the detailed technical metadata for any of them?

---

**👤 You:**
> "Show the latest SEO audit results for 'example.com'."

**🤖 AI Agent:**
> Audit intelligence orchestrated! For example.com, I've identified a high-fidelity health score of 85%. There are 10 technical issues flagged, including 5 broken links. I've retrieved the technical step metadata for your review. Need help prioritizing the fixes?

---

**👤 You:**
> "Check for any keywords with significant rank drops this week."

**🤖 AI Agent:**
> Operational monitoring orchestrated! I've identified 3 high-fidelity keywords with rank drops greater than 5 positions, including 'AI Tools'. I've retrieved the technical SERP metadata for your review. Shall I check for any corresponding site health changes?


## ❓ FAQ

**Q: How do I find my Raven Tools API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique Access Token from the credentials section.

**Q: Can I check keyword rankings via AI?**
Yes! The `list_raven_keywords` tool allows your agent to retrieve high-fidelity position metadata for all tracked search terms.

**Q: How do I list my active projects?**
Use the `list_raven_projects` tool to retrieve your complete high-fidelity directory along with the unique identifiers for all managed SEO campaigns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/raven-tools](https://vinkius.com/mcp/raven-tools)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Raven Tools** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `raven-tools` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Raven Tools** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "raven-tools": {
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
