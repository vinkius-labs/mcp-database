# Google Ads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-ads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor and analyze Google Ads performance — track campaigns, keywords, and metrics via AI.

## Description
Connect your **Google Ads** account to your AI agent and gain real-time visibility into your advertising performance. Use natural language to audit campaigns, analyze keyword efficiency, and retrieve performance reports across your entire account.

### What you can do

- **Campaign Monitoring** — List all active campaigns, check their status, and deep-dive into specific configuration settings
- **Ad Group & Ad Analysis** — Explore ad groups and individual ads to understand your account structure and creative performance
- **Performance Reporting** — Fetch detailed metrics (clicks, impressions, cost, conversions) for any date range through simple queries
- **Keyword Insights** — Search for specific keywords and analyze their individual performance metrics to optimize your bidding strategy
- **Account Overviews** — Get a high-level summary of your account's health and budget consumption across all accessible customers

### How it works

1. Subscribe to this server
2. Enter your Google Ads Customer ID and Developer Token
3. Complete the secure Google OAuth flow to authorize access
4. Start analyzing your ad performance from Claude, Cursor, or any MCP-compatible client

Stop wrestling with complex reporting dashboards. Your AI agent acts as your dedicated PPC specialist, providing insights instantly.

### Who is this for?

- **Marketing Managers** — quickly check daily spend and conversion volume across multiple campaigns without opening the Ads UI
- **PPC Specialists** — audit keyword performance and identify low-performing ads through conversational queries
- **Agency Leads** — monitor performance across multiple client accounts and generate fast executive summaries


## Available Tools
- **get_account_summary**: Get an overview of the account performance
- **get_ad_performance**: Get performance metrics for ads in an ad group
- **get_change_status**: Check recent changes in the account
- **get_campaign_details**: Get detailed settings for a campaign
- **get_campaign_report**: Fetch performance metrics for campaigns
- **get_keyword_performance**: Get performance metrics for keywords in an ad group
- **list_accessible_customers**: List accessible Google Ads customer accounts
- **list_ad_groups**: List ad groups within a campaign
- **list_ads**: List ads within an ad group
- **list_budgets**: List account budgets
- **list_campaigns**: List all Google Ads campaigns
- **search_keywords**: Search for keywords and their performance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Ads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active campaigns and their current status."

**🤖 AI Agent:**
> Fetching campaigns... You have 5 active campaigns. 'Summer Sale 2024' is currently 'ENABLED', while 'Retargeting - Q2' is 'PAUSED'. Would you like the performance report for the 'Summer Sale' campaign?

---

**👤 You:**
> "How many clicks and conversions did we get in the last 7 days?"

**🤖 AI Agent:**
> Running account summary... In the last 7 days, your account recorded 1,240 clicks and 45 conversions across all campaigns. The total cost was approximately $850.30.

---

**👤 You:**
> "Show me the top performing keywords in ad group 93021."

**🤖 AI Agent:**
> Analyzing keyword performance... In ad group 93021, the keyword 'best running shoes' has the highest CTR at 5.2%, followed by 'lightweight trainers' at 4.8%. Would you like to see the average CPC for these keywords?


## ❓ FAQ

**Q: Can I pause or enable campaigns directly through the AI agent?**
Currently, the tools focus on investigative queries and performance analysis. To change the status of a campaign or ad group, please use the Google Ads UI to ensure full budget and policy compliance.

**Q: How can I check which keywords are driving the most conversions?**
You can use the `getKeywordPerformance` tool for a specific ad group. It will return metrics like clicks, impressions, and CTR for each keyword, allowing the AI to identify your top contributors.

**Q: Does this integration support multiple client accounts under a manager account?**
Yes! Use the `list_accessible_customers` tool to see all accounts your credentials have access to. You can then specify the target Customer ID when running performance queries.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-ads](https://vinkius.com/mcp/google-ads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Ads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-ads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Ads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-ads": {
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
