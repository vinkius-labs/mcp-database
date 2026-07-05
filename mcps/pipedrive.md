# Pipedrive MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedrive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate sales CRM via Pipedrive — manage deals, persons, and activities directly from any AI agent.

## Description
Connect your **Pipedrive** account to any AI agent and take full control of your sales orchestration and pipeline management through natural conversation. Pipedrive is the leading CRM for sales teams, and this integration allows you to retrieve deal metadata, update customer records, and monitor activity logs directly from your chat interface.

### What you can do

- **Deal & Pipeline Orchestration** — List all managed deals and retrieve detailed metadata programmatically across various pipelines and stages to ensure your sales velocity is always synchronized.
- **Contact & Organization Intelligence** — Access and monitor your centralized database of persons and organizations directly from the AI interface to maintain high-fidelity customer profiles.
- **Activity & Workflow Control** — List and create sales activities (calls, meetings, tasks) via natural language to drive better team productivity and follow-up efficiency.
- **Sales Search & Discovery** — Perform targeted searches for specific deals or contacts to maintain a clear overview of your opportunities using simple AI commands.
- **Operational Monitoring** — Track system responses and manage user account metadata to ensure your sales workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pipedrive API Token from your personal preferences
3. Start managing your sales CRM from Claude, Cursor, or any MCP-compatible client

No more manual logging into the CRM to check deal status. Your AI acts as a dedicated sales assistant or pipeline coordinator.

### Who is this for?

- **Sales Representatives** — quickly retrieve deal summaries and monitor next activities without switching apps.
- **Account Managers** — automate the management of client records and track interaction history via natural conversation.
- **Sales Operations Teams** — streamline the retrieval of pipeline metadata and monitor organizational health directly within the chat.


## Available Tools (12)
- **list_sales_deals**: List CRM deals
- **list_crm_organizations**: List client companies
- **list_crm_persons**: List individual contacts
- **list_sales_pipelines**: List sales workflows
- **list_pipeline_stages**: List workflow stages
- **search_deals_by_name**: Find deals
- **create_new_deal**: Add new deal
- **get_api_status**: Check connection
- **get_deal_details**: Get deal info
- **get_organization_details**: Get company info
- **get_person_details**: Get contact info
- **list_user_activities**: List tasks and meetings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipedrive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my open deals in Pipedrive."

**🤖 AI Agent:**
> I've retrieved your open deals. You have 4 active opportunities including 'Acme Corp Upgrade' and 'Globex Renewal'. Would you like to see the next activity for any of them?

---

**👤 You:**
> "Show me all deals in the negotiation stage with a value above $50,000 and their expected close dates."

**🤖 AI Agent:**
> 8 deals in Negotiation stage above $50K. "Acme Corp Platform License" at $185,000 expected to close May 28th (85% probability). "TechVentures Annual Contract" at $92,000 closing June 5th. "ScaleUp Enterprise Deal" at $78,000 has been in negotiation for 23 days. "DataFlow Migration" at $67,000 needs a follow-up call. Total pipeline value in negotiation: $724,000.

---

**👤 You:**
> "Add a new activity to schedule a demo call with contact Maria Chen at Meridian Corp for next Tuesday."

**🤖 AI Agent:**
> Activity created successfully. Type: Demo Call. Contact: Maria Chen (VP Engineering, Meridian Corp). Scheduled: Tuesday, May 20th at 2:00 PM EST. Duration: 45 minutes. Linked to deal "Meridian Corp Enterprise" ($125,000). Calendar invitation sent to maria.chen@meridian.io. A reminder has been set for 1 hour before the call.


## ❓ FAQ

**Q: Can my AI automatically find a specific deal by its ID?**
Yes! Use the `get_deal` tool with the Deal ID. Your agent will respond with complete metadata, including value, status, pipeline stage, and associated contacts in seconds.

**Q: How do I find my Pipedrive API Token?**
Log in to Pipedrive, click on your profile icon at the top right, navigate to **Personal preferences** > **API**, and you will find your unique secret token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedrive](https://vinkius.com/mcp/pipedrive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipedrive** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipedrive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipedrive** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipedrive": {
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
