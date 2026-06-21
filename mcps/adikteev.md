# Adikteev MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adikteev)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

App retargeting and churn prediction — manage audience segments and track campaign performance via AI.

## Description
Connect your **Adikteev** account to your AI agent to unlock professional app retargeting and user retention insights. From managing custom audience segments to monitoring campaign performance and retrieving churn probability scores, your agent handles your mobile growth ecosystem through natural conversation.

### What you can do

- **Audience Orchestration** — List, create, and manage audience segments for targeted app retargeting campaigns
- **Performance Reporting** — Retrieve detailed campaign performance data to monitor ROI and engagement metrics
- **Churn Prediction** — Access churn probability scores to identify at-risk app users before they leave your ecosystem
- **Company Insights** — List companies and retrieve technical metadata required for audience management
- **Growth Monitoring** — Quickly audit your retargeting efforts and identify high-value user segments directly from chat

### How it works

1. Subscribe to this server
2. Enter your Adikteev API credentials (email and password)
3. Start managing your app retargeting and tracking user retention through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Marketers** — automate audience segment management and campaign performance audits
- **User Retention Specialists** — retrieve churn scores to trigger personalized re-engagement workflows
- **UA Managers** — monitor retargeting ROI and identify the most profitable user segments
- **Data Analysts** — pull historical campaign data into your B2B intelligence tools effortlessly


## Available Tools
- **list_companies**: Retrieve your company ID
- **list_segments**: List audience segments
- **create_segment**: Create an audience segment
- **get_churn_scores**: Retrieve user churn scores
- **get_reporting**: Get campaign performance data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adikteev** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all audience segments for my company."

**🤖 AI Agent:**
> I've retrieved your audience segments. You have 5 active segments, including 'Inactive Users (30d)', 'High Value Purchasers', and 'Cart Abandoners'. Would you like to create a new one?

---

**👤 You:**
> "Retrieve the churn scores for my app with bundle 'com.example.app'."

**🤖 AI Agent:**
> I've retrieved the churn score data for bundle 'com.example.app'. I have a list of users ranked by churn probability from 1 to 10. Would you like to identify the users in bucket 10 (highest risk)?

---

**👤 You:**
> "Show me the performance of my retargeting campaigns."

**🤖 AI Agent:**
> I've pulled the reporting data. Your active retargeting campaigns have reached 50,000 users with an average re-engagement rate of 12%. Would you like to see the ROI for a specific campaign?


## ❓ FAQ

**Q: How do I get my Adikteev API account?**
You must contact your Adikteev Account Manager to have them enable API access for your account. Once enabled, you can use your standard login credentials (email and password) to authorize the agent.

**Q: What is a Churn Score?**
A churn score ranks app users by their probability of leaving. Adikteev provides these in 'buckets' from 1 to 10, where 10 represents the highest risk of churn.

**Q: How do I create a new audience segment?**
Use the `create_segment` tool and provide your `companyId`, a name, and a description. Your agent will create the segment in Adikteev and provide a `segmentId` for device ID uploads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adikteev](https://vinkius.com/mcp/adikteev)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adikteev** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `adikteev` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adikteev** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adikteev": {
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
