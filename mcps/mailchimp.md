# Mailchimp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailchimp)
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


## Available Tools
- **add_member**: Pass status (subscribed, unsubscribed, cleaned, pending, transactional).

Add a new contact to a Mailchimp audience
- **list_audiences**: List all Mailchimp audiences (lists). Returns audience IDs, names, member counts, and stats
- **list_automations**: List all automation workflows in the account
- **list_campaigns**: Can be used to find a campaign ID.

List Mailchimp campaigns. Returns campaign IDs, types, subjects, send times, and open/click stats
- **create_campaign**: Create a new Mailchimp campaign. Returns campaign ID
- **delete_member**: Requires the list_id and the subscriber MD5 hash (lowercase MD5 of the email).

Archive/remove a subscriber from an audience
- **get_audience**: Only use this when you need detailed statistics or configuration.

Get details of a Mailchimp audience. Returns name, member count, open/click rates, and merge fields configuration
- **get_campaign**: Get full details of a Mailchimp campaign
- **list_members**: Requires an audience ID.

List members (contacts) in a Mailchimp audience. Returns email addresses, status, and tags
- **get_report**: Get Mailchimp campaign performance report
- **search_members**: Search Mailchimp contacts across all audiences by name or email
- **list_segments**: List saved segments for an audience
- **send_campaign**: This action is irreversible. Triggers live email send.

Send a Mailchimp campaign immediately
- **update_member**: Pass json_body with fields like status, merge_fields, tags, etc.

Update subscriber information in an audience


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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailchimp](https://vinkius.com/mcp/mailchimp)
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
3. Set Type to "SSE", enter `mailchimp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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
