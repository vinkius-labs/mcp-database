# Agency Elephant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agency-elephant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track insurance agency performance, manage agent commissions, and monitor policy renewals for better business intelligence.

## Description
Connect your **Agency Elephant** account to any AI agent and take full control of your insurance lead management and automated sales sequences through natural conversation.

### What you can do

- **Lead & Record Orchestration** — List and manage your entire insurance lead database programmatically, retrieving detailed high-fidelity profiles and historical interaction metadata
- **Automated Drip Intelligence** — Programmatically trigger SMS and Email drip sequences for specific leads to maintain a perfectly coordinated follow-up pipeline
- **Pipeline & Group Architecture** — Access and monitor your lead organization structure, including pipelines and custom groups, to ensure perfectly coordinated team focus
- **Engagement Monitoring** — Access high-fidelity lead summaries and track campaign performance directly through your agent for instant operational reporting
- **Team Visibility** — Retrieve complete directories of workspace users and coordinate assignments across your agency directly through your chat interface

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Agency Elephant dashboard (Account Settings > Integrations)
3. Start orchestrating your insurance sales pipeline from Claude, Cursor, or any MCP client

No more manual toggling between CRM tabs or missing critical follow-ups. Your AI acts as your dedicated sales coordinator and lead architect.

### Who is this for?

- **Insurance Agents** — instantly retrieve lead details and trigger follow-up sequences using natural language commands
- **Agency Managers** — monitor team pipeline health and coordinate lead distribution without leaving your workspace
- **Sales Operations** — automate the ingestion of new leads into specialized drip campaigns through simple AI queries


## Available Tools (8)
- **add_lead_to_group**: Add a lead to a group
- **create_lead**: Create a new lead
- **get_lead_details**: Get lead details
- **list_campaigns**: List all campaigns
- **list_lead_groups**: List all lead groups
- **list_leads**: List all leads
- **list_workspace_users**: List all team members
- **trigger_drip_campaign**: Start a drip campaign for a lead


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agency Elephant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active users in my Agency Elephant workspace."

**🤖 AI Agent:**
> I've retrieved your workspace users. You currently have 5 active team members, including 'Sarah Manager' and 'Mike Agent'. Would you like the detailed metadata for any of them?

---

**👤 You:**
> "Trigger the 'New Prospect Follow-up' campaign (ID: 'camp_123') for lead ID '90210'."

**🤖 AI Agent:**
> Campaign triggered! I've successfully enrolled lead 90210 into the 'New Prospect Follow-up' sequence. They will receive the first SMS automated update shortly. Need help monitoring the delivery status?

---

**👤 You:**
> "Create a new lead 'John Doe' (john@example.com) with phone '+15550123'."

**🤖 AI Agent:**
> Lead orchestrated! I've successfully registered John Doe (ID: lead_789) in your CRM. He is now active and ready for assignment to a pipeline or campaign. Shall I list your available groups for him?


## ❓ FAQ

**Q: How do I find my Agency Elephant API Key?**
Log in to your account, navigate to **Account Settings** > **Integrations**, and copy your unique API Key from the credentials section.

**Q: Can I add a lead to a specific group via AI?**
Yes! The `add_lead_to_group` tool allows your agent to categorize leads programmatically by providing the lead ID and target group ID.

**Q: How do I trigger an automated drip campaign?**
Use the `trigger_drip_campaign` tool and provide the lead ID along with the campaign ID you want to initialize programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agency-elephant](https://vinkius.com/mcp/agency-elephant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agency Elephant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agency-elephant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agency Elephant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agency-elephant": {
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
