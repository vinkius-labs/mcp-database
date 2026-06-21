# Grepsr MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grepsr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate web scraping via Grepsr — manage reports, trigger crawls, and retrieve data directly via AI.

## Description
Connect your **Grepsr** account to any AI agent and take full control of your managed web scraping operations. Use natural language to trigger on-demand crawls, monitor data delivery schedules, and retrieve structured datasets directly into your workflow.

### What you can do

- **Report Orchestration** — List all your reports and crawlers and retrieve specific configuration details natively
- **Live Data Retrieval** — Query and resolve structured records from specific reports or run histories flawlessly
- **On-Demand Crawling** — Trigger manual crawl runs for any report to refresh your datasets synchronously
- **Execution Monitoring** — Track the status and record counts of crawl histories to audit data quality flawlessly
- **Webhook Management** — Setup and audit webhooks to notify your internal systems as soon as new data is ready natively
- **Integration Visibility** — List active data delivery integrations including S3, SFTP, and cloud storage providers synchronously

### How it works

1. Subscribe to this server
2. Enter your Grepsr API Key (found in your Grepsr account under Profile > Personal Details)
3. Start managing your data extraction pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Engineers** — quickly check crawl statuses and verify record counts without manual dashboard navigation
- **Market Researchers** — trigger data refreshes for competitor pricing or product lists directly through the chat interface
- **Operations Teams** — retrieve the latest scraped datasets and verify delivery integration status synchronously


## Available Tools
- **create_webhook**: Configure a new webhook URL for a report
- **get_me**: Get details for the current Grepsr account
- **get_latest_data**: Retrieve the most recent scraped dataset for a report
- **get_report_data**: Query scraped records from a specific report
- **get_report_details**: Get metadata and configuration for a specific report
- **get_report_history**: Retrieve the execution history (runs) for a specific report
- **get_usage_stats**: Check account API usage and request limits
- **list_integrations**: List active data delivery integrations (e.g. S3, SFTP)
- **list_projects**: List all scraping projects
- **list_reports**: List all reports and crawlers in your Grepsr account
- **list_webhooks**: List webhooks configured for a specific report
- **run_report**: Trigger an on-demand crawl for a specific report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grepsr** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my web scraping reports in Grepsr"

**🤖 AI Agent:**
> Retrieving your reports... I found 3 active crawlers: 'Amazon Product Data' (ID: 104), 'LinkedIn Jobs' (ID: 105), and 'Real Estate Listings' (ID: 108). Would you like to see the latest data for any of these?

---

**👤 You:**
> "Trigger a manual crawl for report ID 104"

**🤖 AI Agent:**
> Starting crawl... Success! I've triggered a manual run for 'Amazon Product Data' (ID: 104). The status is now 'In Progress'. I can check back in a few minutes to see when the data is ready.

---

**👤 You:**
> "Show me the 5 most recent records from the 'Real Estate Listings' report"

**🤖 AI Agent:**
> Fetching records... Here are the 5 latest items from your real estate crawler:
1. 123 Main St - $450,000
2. 456 Oak Ave - $320,000
3. 789 Pine Rd - $580,000
4. 101 Lake Dr - $950,000
5. 202 Hill Ct - $275,000


## ❓ FAQ

**Q: Can my agent trigger a new web crawl in Grepsr?**
Yes. Use the 'run_report' tool. By providing the Report ID, the agent can programmatically trigger an on-demand crawl, starting the data extraction process immediately flawlessly.

**Q: How do I retrieve the actual scraped data records via chat?**
You can use the 'get_report_data' or 'get_latest_data' tools. Your agent will fetch the structured records from Grepsr's database and present them in a readable format within your chat interface flawlessly.

**Q: Can I check my API usage limits through the agent?**
Absolutely. Use the 'get_usage_stats' tool. Your agent will retrieve your current plan limits and remaining API credits, helping you manage your data extraction budget flawlessly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grepsr](https://vinkius.com/mcp/grepsr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Grepsr** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `grepsr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Grepsr** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "grepsr": {
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
