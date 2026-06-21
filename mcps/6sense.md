# 6sense MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/6sense)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Account-based marketing intelligence — identify anonymous visitors, enrich company data, and track intent via AI.

## Description
Connect your **6sense** enterprise account to your AI agent to unlock deep account-based marketing (ABM) insights. From identifying anonymous website traffic to scoring account intent and buying stages, your agent manages B2B intelligence through natural conversation.

### What you can do

- **Company Identification** — Identify anonymous companies visiting your website via IP address analysis
- **Data Enrichment** — Retrieve detailed firmographics and technographics for any account or email address
- **Intent Scoring** — Access AI-driven intent scores (0-100) to prioritize high-value accounts
- **Buying Stages** — Monitor journey stages (Target, Awareness, Consideration, Decision, Purchase) for your target accounts
- **Segment Membership** — Check which marketing segments an account belongs to for better personalization

### How it works

1. Subscribe to this server
2. Enter your 6sense API Token
3. Start prioritizing and enriching your B2B accounts through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Revenue Operations** — automate data flow between 6sense and other sales tools
- **SDRs & BDRs** — research prospect accounts and intent levels before outreach
- **Marketing Managers** — identify which accounts are most engaged with your web content
- **Sales Leaders** — monitor pipeline health and target account journey progress


## Available Tools (4)
- **identify_company**: Identify a company via visitor IP address
- **enrich_company**: g. microsoft.com).

Enrich firmographics and technographics for a domain
- **enrich_person**: Enrich profile information for an email address
- **list_segments**: List marketing segments for a given company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **6sense** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Identify the company for this IP address: 8.8.8.8"

**🤖 AI Agent:**
> I've analyzed the IP address. It belongs to Google (Alphabet Inc.). Their current intent score is 95 and they are in the 'Purchase' journey stage for your product profile.

---

**👤 You:**
> "Enrich the company data for 'tesla.com'."

**🤖 AI Agent:**
> I've retrieved the data for Tesla, Inc. They are in the Automotive & Energy industry, with over 100,000 employees. They use technologies like Splunk and New Relic. Their intent score is currently 82.

---

**👤 You:**
> "Check which 6sense segments 'microsoft.com' belongs to."

**🤖 AI Agent:**
> Microsoft is currently part of 4 segments: 'Tier 1 Enterprise', 'High Intent - Cloud Solutions', 'Existing Customers', and 'Q4 Expansion Targets'.


## ❓ FAQ

**Q: Can I identify which company is visiting my website?**
Yes. By using the `identify_company` tool with a visitor's IP address, 6sense identifies the associated company and provides its intent score and profile data.

**Q: What kind of data can I get for a company domain?**
The `enrich_company` tool retrieves deep firmographics (industry, revenue, employee count), technographics (software they use), and current intent scores for any domain.

**Q: How do I find which segments an account belongs to?**
Use the `list_segments` tool with the company domain. It will return all 6sense marketing segments the account is currently part of, allowing for personalized outreach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/6sense](https://vinkius.com/mcp/6sense)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **6sense** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `6sense` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **6sense** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "6sense": {
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
