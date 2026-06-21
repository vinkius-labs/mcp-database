# PartnerPortal.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/partnerportalio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage your partner and reseller programs with deal registration, lead sharing, and performance tracking for channel sales.

## Description
Connect your **PartnerPortal.io** account to any AI agent and take full control of your channel sales orchestration and partner relationship management through natural conversation. PartnerPortal.io provides a comprehensive platform for scaling partner ecosystems, and this integration allows you to retrieve lead metadata, monitor active deals, and manage partner accounts directly from your chat interface.

### What you can do

- **Lead & Opportunity Orchestration** — List, create, and update leads programmatically across your partner network to ensure your sales pipeline is always synchronized.
- **Partner & Account Intelligence** — Access and monitor partner profiles and account-level metadata directly from the AI interface to maintain high-fidelity relationships.
- **Deal Lifecycle Control** — Access and monitor deal statuses via natural language to track channel revenue growth and partner performance.
- **Schema & Metadata Oversight** — Retrieve object schemas and list account roles using simple AI commands to ensure your data mapping is always optimized.
- **Operational Monitoring** — Track system responses and manage bulk creation jobs to ensure your partner operations are always high-performing.

### How it works

1. Subscribe to this server
2. Enter your PartnerPortal.io API Token (Bearer Token) from your dashboard
3. Start managing your partner program from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the portal. Your AI acts as a dedicated channel manager or partnership coordinator.

### Who is this for?

- **Channel Managers** — quickly retrieve partner performance summaries and monitor lead volume without switching apps.
- **Partnership Teams** — automate the creation of new leads and track deal progress via natural conversation.
- **Operations Leads** — streamline the retrieval of account metadata and monitor organizational partnership health directly within the chat.


## Available Tools
- **check_api_status**: Verify API connectivity and account status
- **create_lead**: Create a new lead
- **get_account**: Get details for a specific account
- **get_deal**: Get details for a specific deal
- **get_lead**: Get details for a specific lead
- **get_partner**: Get details for a specific partner
- **list_accounts**: List accounts in PartnerPortal.io
- **list_deals**: List deals in PartnerPortal.io
- **list_leads**: io.

List leads in PartnerPortal.io
- **list_partners**: List partners in PartnerPortal.io
- **update_lead**: Update an existing lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PartnerPortal.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active leads for company ID 12345."

**🤖 AI Agent:**
> I've retrieved your leads for company 12345. You have 8 active opportunities including 'Acme Corp Upgrade' and 'New Partnership'. Would you like to see the status of any of them?

---

**👤 You:**
> "Show me all partner organizations and their deal registration pipeline."

**🤖 AI Agent:**
> You have 34 active partner organizations. Top 5 by deal value: "Meridian Solutions" ($890K in pipeline, 12 active deals), "CloudBridge Partners" ($720K, 8 deals), "TechAlliance" ($540K, 15 deals), "Digital Edge" ($430K, 6 deals), and "NextGen IT" ($380K, 9 deals). Total partner pipeline: $4.2M across 67 registered deals.

---

**👤 You:**
> "Register a new lead from partner Meridian Solutions for the Acme Corp enterprise opportunity."

**🤖 AI Agent:**
> Lead registered successfully (ID: lead_4892). Partner: Meridian Solutions. Account: Acme Corp. Opportunity: Enterprise Platform Migration, estimated value $185,000. Status: Pending Approval. The partner manager has been notified for deal validation. Expected close date set to Q3 2025 based on the partner's estimate.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific lead by its ID?**
Yes! Use the `get_lead` tool with the Company ID and Lead ID. Your agent will respond with complete metadata, including lead status, source, and associated deal info in seconds.

**Q: How do I find my PartnerPortal.io API Token?**
Log in to your PartnerPortal.io account, navigate to **Settings** > **API**, and you will find or generate your unique secret token there. Ensure you have the required plan level for API access.

**Q: What is the Company ID?**
The Company ID is a unique identifier for your organization profile within PartnerPortal.io. You can find it in your portal settings or URL after logging in.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/partnerportalio](https://vinkius.com/mcp/partnerportalio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PartnerPortal.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `partnerportalio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PartnerPortal.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "partnerportalio": {
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
