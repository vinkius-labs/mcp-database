# Merge (Unified Integration API) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/merge-unified-integration-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage unified B2B data via Merge — list HRIS employees, ATS candidates, CRM contacts, and support tickets.

## Description
Connect your **Merge.dev** account to any AI agent and take full control of your unified B2B integrations across HRIS, ATS, CRM, and Ticketing through natural conversation.

### What you can do

- **HRIS Orchestration** — List all active employees and organizational companies from your connected HRIS (e.g., BambooHR, Workday, HiBob) directly from your agent
- **ATS Talent Pipeline** — Retrieve recruited candidates and tracked job applications from your ATS integration (e.g., Greenhouse, Lever, Ashby) to monitor hiring workflows
- **CRM Contact Management** — Access external sales contacts and customer accounts from your CRM (e.g., Salesforce, HubSpot, Pipedrive) to manage your business directory securely
- **Ticketing & Support** — List inbound and outbound support tickets from your issue-tracking boards (e.g., Zendesk, Jira, Front) to stay updated on customer issues
- **Unified Data Access** — Retrieve standardized data structures across hundreds of different integrations using a single set of API tools natively handled by Merge
- **Integration Audit** — Inspect linked account details and meta-configurations to understand the current state and boundaries of your connected workspace securely

### How it works

1. Subscribe to this server
2. Enter your Merge API Key and specific Account Token
3. Start managing your unified B2B data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — audit customer integration health and verify unified data mappings through natural conversation without manual API logging
- **Software Developers** — test unified data responses and verify standardized schemas across multiple categories directly from your workspace
- **RevOps & HR Teams** — retrieve rapid summaries of employees, candidates, or sales contacts across different platforms efficiently


## Available Tools (8)
- **list_employees**: Be aware the list might be paginated or heavy.

List employees from the linked HRIS integration
- **list_companies**: List companies mapped inside the HRIS integration
- **list_candidates**: List recruited candidates across the ATS integration
- **list_applications**: List job applications inside the ATS integration
- **list_contacts**: List external contacts mapped in the CRM integration
- **list_accounts**: List customer accounts parsed from the CRM integration
- **list_tickets**: List inbound/outbound support tickets inside the Ticketing integration
- **get_account_details**: dev.

Retrieve linked Account Details exposing integration boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Merge (Unified Integration API)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active employees from our linked HRIS"

**🤖 AI Agent:**
> Retrieving employee data… I've identified 125 active employees in your HRIS. Highlights include Alex Smith (Software Engineer), Sarah Johnson (Marketing Manager), and Mark Rivera (Product Designer). Would you like the full profile details for any department?

---

**👤 You:**
> "Show me the last 5 candidates in our ATS talent pipeline"

**🤖 AI Agent:**
> Retrieving candidates… I've identified the 5 most recent additions: 1) Jamie Lann (Senior Dev), 2) Riley Vane (UX Lead), 3) Casey Wright, 4) Jordan Bell, and 5) Taylor Reed. I can check the status of their active applications if you'd like.

---

**👤 You:**
> "List all open support tickets in our ticketing integration"

**🤖 AI Agent:**
> I've retrieved your open support tickets. There are 12 active issues, including 'Login Loop Bug' (Priority: High), 'Pricing Question' (Priority: Med), and 'API Auth Error'. Would you like me to extract the full metadata for the high-priority bug?


## ❓ FAQ

**Q: Which integrations does Merge support through the unified API?**
Merge supports over 150+ integrations across HRIS (BambooHR, Workday), ATS (Lever, Greenhouse), CRM (Salesforce, HubSpot), and Ticketing (Zendesk, Jira). Your agent can access all of them using the same standardized tools once the accounts are linked in Merge.

**Q: How do I target a specific customer's data through the agent?**
Each request requires a `MERGE_ACCOUNT_TOKEN` which uniquely identifies a linked account (e.g., a specific customer's integration). By providing this token along with your API key, your agent can retrieve data exclusively from that customer's connected platform.

**Q: Can my agent list candidates from my ATS and support tickets from Zendesk at the same time?**
Yes. Since Merge unifies multiple categories, your agent can use the `list_candidates` and `list_tickets` tools in the same conversation to bridge data from different functional areas of your business instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/merge-unified-integration-api](https://vinkius.com/mcp/merge-unified-integration-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Merge (Unified Integration API)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `merge-unified-integration-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Merge (Unified Integration API)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "merge-unified-integration-api": {
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
