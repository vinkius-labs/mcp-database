# Proxycurl (LinkedIn Data) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/proxycurl-linkedin-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Enrich company and professional data via Proxycurl — lookup websites, funding history, employee profiles, and competitive intelligence directly from your AI agent.

## Description
Connect **Proxycurl** to your AI agent to access real-time B2B intelligence and LinkedIn-derived data. This server provides a powerful suite of tools for sales, recruitment, and market research.

### What you can do

- **Company Intelligence** — Resolve company names to websites, fetch logos, and retrieve deep metadata including industry and leadership using `company_website_lookup` and `get_company_details`.
- **Financial Insights** — Access complete funding histories, investment rounds, and participating investors for private and public companies via `get_company_funding`.
- **People Data** — Enrich professional profiles from work emails or names with `get_employee_profile`, and search for employees within specific organizations using `search_employees`.
- **Market Analysis** — Identify competitors based on product similarity with `get_competitor_listing` and list probable customers or partners.
- **Monitoring** — Create and manage monitor feeds to track organizational changes over time using `create_monitor_feed`.

### How it works

1. Subscribe to this server
2. Enter your Proxycurl API Key
3. Start querying B2B data from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales & RevOps** — Automate lead enrichment and find decision-makers without manual searching.
- **Recruiters** — Identify talent pools and enrich candidate profiles instantly.
- **Market Researchers** — Map out competitive landscapes and track company growth metrics.


## Available Tools (18)
- **add_monitor_target**: Add a target to an existing monitor feed
- **check_disposable_email**: Detect temporary or throwaway email addresses
- **get_company_details**: Retrieve comprehensive company metadata and leadership teams
- **get_company_employee_count**: Retrieve the estimated headcount range for a company
- **get_company_funding**: It may take up to 5 minutes.

Retrieve full funding history, rounds, and participating investors
- **get_company_logo**: Retrieve a 128x128 PNG logo URL for any company
- **get_company_updates**: Aggregate blog posts and X/Twitter updates into a mixed timeline
- **company_website_lookup**: Resolve a company name to its canonical website URL
- **get_competitor_listing**: Find competitors and the reasoning (keyword overlap or product similarity)
- **create_monitor_feed**: Create a new monitor feed for company changes
- **get_customer_listing**: Get a list of probable customers, investors, and partner platforms
- **get_employee_profile**: Enrich professional profiles from work emails or name/employer combinations
- **get_monitor_rss**: Get the RSS feed for a specific monitor feed
- **list_monitor_feeds**: List all active monitor feeds
- **lookup_work_email**: Best-effort lookup of a public work email from a name and domain
- **search_employees**: Find current employees of a company by role and geography
- **get_similar_employees**: Repeat queries are served free from cache.

Find counterparts in similar roles at competing companies
- **get_credit_balance**: Check your remaining API credit balance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Proxycurl (LinkedIn Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the official website for 'Nvidia'."

**🤖 AI Agent:**
> I've looked it up. The canonical website for Nvidia is 'https://www.nvidia.com'. I can now use this URL to fetch more details like funding or employee counts if you'd like.

---

**👤 You:**
> "Show me the funding history for 'SpaceX'."

**🤖 AI Agent:**
> Fetching funding data... SpaceX has an extensive history including multiple Series rounds. Notable investors include Fidelity, Google, and Founders Fund. Would you like a breakdown of the most recent round?

---

**👤 You:**
> "Who are the main competitors for 'Zoom'?"

**🤖 AI Agent:**
> Searching for competitors... Based on product similarity and market overlap, key competitors for Zoom include Microsoft (Teams), Cisco (Webex), and Google (Meet). I can also provide a customer listing for Zoom if needed.


## ❓ FAQ

**Q: How do I find a company's official website if I only have their name?**
Use the `company_website_lookup` tool. It resolves a company name to its canonical URL, which is the primary identifier needed for most other company-related tools.

**Q: Can I see who invested in a specific startup?**
Yes. The `get_company_funding` tool provides a detailed history of funding rounds, including the amounts raised and the names of participating investors.

**Q: Is it possible to get professional details from just a work email?**
Absolutely. Use the `get_employee_profile` tool with the `work_email` parameter to retrieve enriched professional data, including current role and employer information.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/proxycurl-linkedin-data](https://vinkius.com/mcp/proxycurl-linkedin-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Proxycurl (LinkedIn Data)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `proxycurl-linkedin-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Proxycurl (LinkedIn Data)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "proxycurl-linkedin-data": {
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
