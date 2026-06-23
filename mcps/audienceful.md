# Audienceful MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/audienceful)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage subscribers, custom fields, and email automations via Audienceful — orchestrate newsletters and campaigns directly via AI.

## Description
Connect your **Audienceful** account to any AI agent and transform how you manage your email marketing and audience data through natural conversation.

### What you can do

- **People Management** — Create, search, and update subscriber profiles and manage their subscription status across your workspace
- **Custom Data Fields** — Define and manage custom data points to segment your audience with surgical precision
- **Automation Triggers** — Programmatically trigger email sequences and marketing automations for specific users or events
- **Performance Auditing** — Query and analyze campaign performance and audience growth metrics without manual exports

### How it works

1. Subscribe to this server
2. Enter your Audienceful API Key
3. Start managing your email marketing workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — instantly manage your newsletter subscribers and check growth stats while writing content
- **Marketing Teams** — trigger complex sequences and update user tags directly from your team's workspace
- **Growth Engineers** — automate the creation of custom fields and data mapping from your IDE


## Available Tools (10)
- **create_custom_field**: Create a new custom field for your audience members
- **create_person**: You must provide at least an email address.

Add a new person to your audience
- **delete_custom_field**: Delete a custom field
- **delete_person**: Use with caution.

Permanently remove a person from your audience
- **get_person**: Get details for a specific person by their UID
- **list_custom_fields**: List all custom fields defined in your audience
- **list_people**: You can filter by status or search for a specific email address.

List all people in your Audienceful audience
- **list_send_reports**: List recent email send reports
- **trigger_automation**: Manually trigger an automation for a person
- **update_person**: Update an existing person profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Audienceful** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for subscribers who have the 'Company' field set to 'TechCorp'."

**🤖 AI Agent:**
> I've scanned your audience. I found 3 subscribers matching 'TechCorp': Sarah L. ([email protected]), Mike R. ([email protected]), and Anna K. ([email protected]). Would you like to tag them all with 'Enterprise'?

---

**👤 You:**
> "Trigger the 'onboarding-welcome' sequence for [email protected]"

**🤖 AI Agent:**
> The automation 'onboarding-welcome' has been successfully triggered for [email protected]. They should receive the first email in the sequence shortly.

---

**👤 You:**
> "List all custom fields currently defined in my Audienceful workspace."

**🤖 AI Agent:**
> I've retrieved your custom data structure. You currently have 5 custom fields defined: 'Company' (company_name), 'Job Title' (job_title), 'Lead Score' (lead_score), 'Referral Source' (ref_source), and 'Last Event' (last_event).


## ❓ FAQ

**Q: Can the AI automatically update a subscriber's custom field values?**
Yes! By using the `update_person` tool, your agent can modify any existing custom field values for a specific subscriber identified by their email or ID in seconds.

**Q: How do I trigger an automation sequence for a new user?**
Simply ask the agent to run the `trigger_automation` action. You'll need to provide the slug of the automation and the target person's email address.

**Q: Does this integration allow for bulk deletion of my entire audience?**
No. The current toolset focuses strictly on managing individual subscriber records and queries. Destructive actions on the entire audience structure are not exposed to ensure your data remains secure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/audienceful](https://vinkius.com/mcp/audienceful)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Audienceful** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `audienceful` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Audienceful** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "audienceful": {
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
