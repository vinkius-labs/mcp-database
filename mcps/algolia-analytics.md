# Algolia Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/algolia-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Search performance intelligence — audit CTR, conversions, and top searches via AI.

## Description
Connect your **Algolia** application to your AI agent to unlock professional search performance orchestration and data intelligence. From monitoring real-time Click-Through Rates (CTR) and Conversion Rates (CR) to auditing top searches without results and analyzing AB test performance, your agent handles your search strategy through natural conversation.

### What you can do

- **Search Performance Auditing** — Retrieve granular metrics for CTR, average click position, and conversion rates across your indices
- **Term Discovery** — List top searches, recent queries, and terms that returned zero results to identify content gaps
- **User Intelligence** — Monitor unique user counts and filter performance to understand your audience's behavior
- **AB Test Monitoring** — List and audit active and historical AB tests to ensure your search optimizations are effective
- **Insights Automation** — Quickly identify search trends or filter performance bottlenecks directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Algolia Application ID and Analytics API Key
3. Start monitoring your search performance and retrieving business insights through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — monitor search relevance and conversion trends to drive roadmap decisions
- **Search Engineers** — audit AB test results and average click positions to optimize ranking algorithms
- **Content Strategists** — identify 'No Result' searches to discover new content opportunities
- **Marketing Analysts** — retrieve granular search engagement data for cross-channel performance reporting


## Available Tools (10)
- **get_click_through_rate**: Get search CTR
- **get_conversion_rate**: Get search conversion rate
- **get_average_click_position**: Get average click rank
- **list_top_searches**: List most popular terms
- **list_no_result_searches**: List failed searches
- **list_no_click_searches**: List ignored searches
- **get_unique_users_count**: Count search users
- **list_recent_searches**: List latest queries
- **list_top_filters**: List popular filters
- **list_ab_tests**: List AB testing status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Algolia Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the Click-Through Rate (CTR) for my 'Products' index for the last 30 days."

**🤖 AI Agent:**
> I've retrieved the CTR for your Products index. Over the last 30 days, your average CTR was 4.2%. The highest peak was 6.5% last Tuesday. Would you like to see the average click position for this period?

---

**👤 You:**
> "List the top 10 searches that returned no results yesterday."

**🤖 AI Agent:**
> I've analyzed yesterday's 'No Result' queries. Your top 10 failed searches include 'limited edition boots', 'smart watch pro', and 'vintage camera'. These represent a combined 500 missed opportunities. Would you like to see the full list?

---

**👤 You:**
> "Show the results of my active AB tests."

**🤖 AI Agent:**
> You have 2 active AB tests. Test 'Ranking Logic V2' shows a 5% increase in conversion rate for the variant group. Test 'Mobile UI Tweak' is currently showing neutral results. Would you like the detailed metrics for the Ranking Logic test?


## ❓ FAQ

**Q: How do I find my Algolia Analytics API Key?**
Log in to the Algolia Dashboard, go to **API Keys**, and look for a key with the `analytics` ACL enabled. You will also need your **Application ID** found on the same page.

**Q: Which region should I choose?**
Algolia Analytics provides region-specific endpoints. Choose **US** for `analytics.us.algolia.com` or **DE** for `analytics.de.algolia.com`. Most applications use the US region by default.

**Q: Why do some metrics show 0 conversion?**
Conversion metrics require you to send events via the **Insights API**. If you aren't currently sending click or conversion events from your frontend, the Analytics API will not have data to report for those metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/algolia-analytics](https://vinkius.com/mcp/algolia-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Algolia Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `algolia-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Algolia Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "algolia-analytics": {
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
