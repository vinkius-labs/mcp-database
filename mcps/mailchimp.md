# Mailchimp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mailchimp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Synchronize marketing contacts — list audiences, control subscriber limits, and edit campaign vectors autonomously.

## Description
Equip any AI agent with robust Mailchimp marketing capabilities. Integrate your mailing operations transparently to control large audiences, tweak contact statuses dynamically, and trigger organizational insights across your campaigns via conversational prompts.

### What you can do

- **Audience (Lists) Syncing** — Target specific segments, pull overall audience IDs, and grasp performance baselines simply
- **Member Administration** — Unsubscribe, fetch, or permanently store subscriber metadata and profile details without web interfaces
- **Campaign Insights** — Map existing drafted or sent emails across campaigns to keep tabs on global performance metrics programmatically

### How it works

1. Enable the MCP connection under your local profile
2. Input an application-level API token specifically derived from your account
3. Engage directly with LLM shells managing flows through raw texts and pure language operations

### Who is this for?

- **Growth Engineers** — pull massive batches of churned lists instantly for re-validation internally directly avoiding manual filtering
- **Content Marketers** — trace campaign statuses quickly when jumping between different platforms constantly


## Available Tools (18)
- **list_audiences**: List Mailchimp audiences. Returns list_id, name, member count
- **list_automations**: List automation workflows. Returns automation_id and status
- **get_campaign**: Get campaign details by campaign_id
- **get_report**: Get campaign report. Returns opens, clicks, bounces, unsubscribes
- **search_members**: Search contacts across all audiences by email or name
- **get_audience**: Get audience details by list_id. Returns stats and settings
- **set_campaign_content**: Set HTML content for a campaign. Required before send/test
- **add_member**: Add contact to audience
- **list_campaigns**: List campaigns. Returns campaign_id, subject, status, send time
- **create_campaign**: Create campaign shell. Returns campaign_id. Set content next
- **delete_member**: Archive contact from audience. Reversible via re-add
- **get_member**: Get single contact by email. Returns status, merge fields, tags
- **list_members**: List contacts in an audience. Returns email, status, tags
- **list_segments**: List segments for an audience. Returns segment_id and conditions
- **send_campaign**: Triggers live delivery.

Send campaign immediately. Irreversible
- **tag_member**: Add/remove tags for a contact
- **test_campaign**: Send test email for a campaign without live delivery
- **update_member**: Update contact fields


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailchimp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the ID of my primary audience list."

**🤖 AI Agent:**
> Query complete. Your main audience 'Weekly Newsletter' uses the List ID 'a1b2c3d4e5'. You can now use this ID to fetch subscribers.

---

**👤 You:**
> "Add exactly test@domain.com as a subscriber to list a1b2c3d4e5."

**🤖 AI Agent:**
> Added subscriber successfully! The contact test@domain.com is now fully mapped as 'subscribed' against that specific audience ID.

---

**👤 You:**
> "List all active marketing campaigns we have on the server."

**🤖 AI Agent:**
> I've fetched 3 campaign items. 'Summer Sale 2026' (Sent), 'Welcome Series' (Draft), and 'Churn Automation' (Sent). Would you like to inspect CTR metrics for the sent ones?


## ❓ FAQ

**Q: Do I need the server prefix combined with my API key automatically?**
Mailchimp API keys usually have a suffix (like `key-us6`). The system will parse everything internally. Just paste the full API key into our simplified authentication box naturally.

**Q: Can I bulk add 5,000 users directly in a single conversational prompt?**
While structurally possible via API logic, context windows prohibit reading arrays of 5000 units. Adding is handled dynamically unit by unit securely or in exceptionally tiny batches to bypass hard egress caps effectively.

**Q: Does the system allow firing off actual live campaigns immediately to massive audiences?**
No. The MCP server prioritizes safe state changes (subscribers). Launching massive destructive dispatches is omitted from the handler array to avoid rogue AI actions firing misconfigured commercial payload sets blindly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mailchimp](https://vinkius.com/ai-agent-connect/mailchimp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mailchimp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailchimp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mailchimp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailchimp": {
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
