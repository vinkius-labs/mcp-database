# Salesmate MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesmate)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate sales CRM via Salesmate — manage contacts, track deals, and log activities directly with AI.

## Description
Connect your **Salesmate** account to any AI agent and take full control of your sales automation and customer relationship orchestration through natural conversation. Salesmate provides a modern and powerful CRM platform, and this integration allows you to retrieve contact metadata, manage deal pipelines, and log real-time sales activities directly from your chat interface.

### What you can do

- **Contact & Relationship Orchestration** — List and create contacts and companies programmatically to ensure your CRM database is always synchronized.
- **Pipeline & Deal Intelligence** — Access and monitor your sales deals and retrieve detailed status metadata directly from the AI interface to close deals faster.
- **Activity & Task Control** — Log calls, meetings, and tasks and retrieve detailed activity history via natural language.
- **Team & User Oversight** — Access team member metadata and monitor system users to ensure your sales team is fully integrated.
- **Operational Monitoring** — Track system activity and monitor webhooks to ensure your automated sales flows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Salesmate Session Token and Link Name (Subdomain) from your account settings
3. Start managing your CRM from Claude, Cursor, or any MCP-compatible client

No more manual CRM entry or pipeline searching. Your AI acts as a dedicated sales operations manager or intelligent account assistant.

### Who is this for?

- **Sales Teams & SDRs** — quickly retrieve customer details and monitor deal statuses without switching apps.
- **Account Managers** — automate the logging of client interactions and track task progress via natural conversation.
- **Operations Teams** — streamline the retrieval of user metadata and monitor CRM health directly within the chat.


## Available Tools (12)
- **create_activity**: Log a new activity
- **create_contact**: Create a new contact
- **create_deal**: Create a new deal
- **get_account_info**: Get current profile
- **get_contact**: Get contact details
- **get_deal**: Get deal details
- **list_activities**: List CRM activities
- **list_contacts**: List all CRM contacts
- **list_deals**: List sales deals
- **list_team_users**: List all team members
- **list_webhooks**: List configured webhooks
- **update_contact**: Update contact info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesmate** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active deals in my Salesmate pipeline."

**🤖 AI Agent:**
> I've retrieved your deals. You have 5 active opportunities including 'Project Alpha' and 'Q4 Renewals'. Which one would you like to update the stage for?

---

**👤 You:**
> "Show me the sales pipeline with deal values grouped by stage and expected close dates."

**🤖 AI Agent:**
> Sales pipeline: $4.2M total value across 67 deals. By stage: Prospecting (18 deals, $890K), Qualification (15, $780K), Proposal (12, $1.1M), Negotiation (8, $680K), Closing (6, $450K), Won this month (8, $320K). Expected to close this month: 14 deals worth $1.13M. Win probability weighted pipeline: $1.8M. Average deal size: $62,700. Sales cycle: 34 days average. Top rep: Sarah Chen with $890K in pipeline. 3 deals are stale (no activity 21+ days).

---

**👤 You:**
> "Create a new deal for Meridian Corp worth $85,000 and assign it to the enterprise sales team."

**🤖 AI Agent:**
> Deal created: "Meridian Corp - Enterprise Platform License". Value: $85,000. Stage: Qualification. Owner: James Park (Enterprise Sales). Contact: David Chen (CTO). Expected close: June 30, 2025. Pipeline: Enterprise. Tags: SaaS, Annual License. Next action: "Discovery call" scheduled for Thursday at 2 PM. Auto-enrichment pulled company data: 340 employees, Series C, San Francisco. Lead score: 87/100. Similar won deals in database: 4 (avg cycle: 28 days).


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific contact just by providing their ID?**
Yes! Use the `get_contact` tool with the Contact ID. Your agent will respond with the complete metadata for the record, including associated deals and communication history in seconds.

**Q: How do I find my Salesmate Access Token and Link Name?**
Log in to your Salesmate account, click on your profile picture > **My Account** > **Access Key**, and you will find your Session Key and Link Name there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesmate](https://vinkius.com/mcp/salesmate)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesmate** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salesmate` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesmate** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesmate": {
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
