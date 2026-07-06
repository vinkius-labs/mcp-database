# Tianyancha / 天眼查 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tianyancha)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Leading enterprise data platform in China — search companies, check industrial info, and monitor risks via AI.

## Description
Empower your AI agent to orchestrate your business intelligence and due diligence with **Tianyancha** (天眼查), the premier enterprise data platform in China. By connecting Tianyancha to your agent, you transform complex industrial research, ownership auditing, and risk monitoring into a natural conversation. Your agent can instantly search for companies, retrieve detailed registration metadata, browse shareholder structures, and monitor industrial abnormalities without you ever needing to navigate the comprehensive Tianyancha portal. Whether you are conducting B2B lead research or auditing potential partners, your agent acts as a real-time business intelligence assistant, keeping your data accurate and your decisions informed.

### What you can do

- **Enterprise Orchestration** — Search for companies and retrieve detailed basic and industrial metadata.
- **Ownership Auditing** — Browse shareholder lists and outward investments to identify corporate structures.
- **Personnel Monitoring** — List main staff and executives to identify key decision-makers within an enterprise.
- **Risk Management** — Retrieve risk indicators, court cases, and industrial abnormalities for any registered company.
- **IP Tracking** — Browse registered trademarks, patents, and copyrights to audit intellectual property assets.

### How it works

1. Subscribe to this server
2. Enter your Tianyancha API Token
3. Start managing your business intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & B2B Leads** — search for potential clients and identify key executives through natural language queries.
- **Legal & Compliance** — conduct due diligence and monitor corporate risks directly from your AI-powered workspace.
- **Business Analysts** — retrieve comprehensive corporate data for market research and competitive analysis.
- **Tianyancha Power Users** — integrate your existing industrial research workflows into your AI-driven daily routines.


## Available Tools (10)
- **get_contact_info**: Get enterprise contact info
- **get_full_details**: Get full enterprise details
- **list_branches**: List company branches
- **list_shareholders**: List company shareholders
- **get_basic_info**: Get enterprise basic info
- **list_investments**: List outward investments
- **list_ip**: List intellectual property
- **list_risks**: List enterprise risk info
- **list_staff**: List main staff/executives
- **search_enterprise**: Enterprise search by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tianyancha / 天眼查** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for companies named 'Alibaba' in Tianyancha."

**🤖 AI Agent:**
> I've retrieved the search results for 'Alibaba'. There are several matches, including 'Alibaba Group Holding Limited' and 'Alibaba Cloud'. Which one would you like the basic information for?

---

**👤 You:**
> "Show me the shareholder structure for 'Huawei'."

**🤖 AI Agent:**
> I've listed the shareholders for Huawei. The primary owner is the Union of Huawei Investment & Holding Co., Ltd. Would you like a list of Huawei's outward investments as well?

---

**👤 You:**
> "Check for any risk information regarding 'Evergrande'."

**🤖 AI Agent:**
> I've retrieved the risk indicators for Evergrande. There are numerous court cases and industrial abnormalities listed. Should I retrieve the details for the most recent legal incidents?


## ❓ FAQ

**Q: How do I find my Tianyancha API Token?**
Log in to the [Tianyancha OpenAPI Platform](https://open.tianyancha.com/), go to [Control Panel] -> [My Interface], and you will find your unique Authorization Token there.

**Q: Is there a limit to the search queries?**
The search limits depend on your Tianyancha OpenAPI subscription plan. Ensure your token has the necessary permissions enabled for the interfaces you want to use.

**Q: Can I check contact information for companies?**
Yes. Use the `get_contact_info` tool with a company name or keyword to retrieve phone numbers, emails, and official addresses registered in the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tianyancha](https://vinkius.com/mcp/tianyancha)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tianyancha / 天眼查** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tianyancha` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tianyancha / 天眼查** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tianyancha": {
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
