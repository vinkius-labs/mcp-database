# SpyFu MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spyfu)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate SEO and PPC research via SpyFu — analyze domain metrics, track keyword stats, and uncover competitor ad history directly from any AI agent.

## Description
Connect your **SpyFu** account to any AI agent and perform deep SEO and PPC competitive analysis through natural conversation.

### What you can do

- **Domain Insights** — Retrieve high-level SEO and PPC metrics, including estimated monthly traffic and ad budgets.
- **Keyword Intelligence** — Get search volume, SEO difficulty, and CPC data for any target keyword.
- **Competitor Mapping** — Identify top organic and paid competitors for any domain to understand the market landscape.
- **Ad History** — View the historical Google Ads copy and performance of your competitors to refine your own strategy.
- **Organic Rankings** — List the specific keywords for which a domain ranks organically in search results.

### How it works

1. Subscribe to this server
2. Enter your SpyFu API Key
3. Start researching domains and keywords from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO Specialists** — quickly audit domain rankings and keyword difficulty without leaving your workflow.
- **Digital Marketers** — analyze competitor ad spend and copy to optimize PPC campaigns.
- **Content Strategists** — identify high-value keywords and organic opportunities based on competitor performance.


## Available Tools (5)
- **get_organic_keywords**: List the keywords for which a domain ranks organically
- **get_ad_history**: View the history of Google Ads run by a competitor
- **get_domain_competitors**: Identify the top organic and paid competitors for a given domain
- **get_domain_overview**: Retrieve high-level SEO and PPC metrics for a specific domain
- **get_keyword_stats**: Get data for specific keywords


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SpyFu** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a domain overview for spyfu.com to see their SEO and PPC metrics."

**🤖 AI Agent:**
> I've retrieved the overview for spyfu.com. They have an estimated monthly organic traffic of 450k visits and a paid budget of approximately $12k/month, ranking for over 80k organic keywords.

---

**👤 You:**
> "What are the keyword stats for 'AI marketing tools' in the US?"

**🤖 AI Agent:**
> For 'AI marketing tools', the search volume is 12,100 per month with an SEO difficulty of 74/100. The estimated CPC is $4.50.

---

**👤 You:**
> "List the top 10 organic keywords for example.com."

**🤖 AI Agent:**
> Here are the top organic keywords for example.com: 1. 'domain examples' (Pos: 1), 2. 'example website' (Pos: 1), 3. 'test domain' (Pos: 2)... [full list provided].


## ❓ FAQ

**Q: Can I see how much a competitor is spending on Google Ads?**
Yes. By using the `get_domain_overview` tool, the agent can retrieve the estimated monthly ad budget for any specific domain.

**Q: How do I find out who the main organic competitors are for a website?**
You can use the `get_domain_competitors` tool with the `type` parameter set to 'organic'. This will return a list of domains competing for the same search results.

**Q: Is it possible to see the actual ad copy used by a competitor in the past?**
Yes, the `get_ad_history` tool allows you to retrieve historical ad copy and performance data for a domain, helping you understand their messaging strategy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spyfu](https://vinkius.com/mcp/spyfu)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SpyFu** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spyfu` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SpyFu** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spyfu": {
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
