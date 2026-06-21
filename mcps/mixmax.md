# Mixmax MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mixmax)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Accelerate your sales cycle with Mixmax — sequences, scheduling, and email tracking.

## Description
Connect **Mixmax** to your AI agent and manage your sales communication through natural conversation. Boost productivity by automating follow-ups and tracking engagement directly from your chat.

### What you can do

- **Sequence Management** — Enroll recipients into automated email sequences and monitor their progress.
- **Smart Scheduling** — Access and share your appointment links and check calendar availability.
- **Email Templates** — List and use your shared snippets to maintain consistent messaging.
- **Engagement Tracking** — Monitor email opens, clicks, and other analytics events in real-time.
- **Task Automation** — Create and manage reminders to never miss a follow-up with a lead.

### How it works

1. Subscribe to this server
2. Enter your Mixmax API Key
3. Start managing your sales outreach with Claude, Cursor, or any MCP client


## Available Tools
- **add_recipient_to_sequence**: Add a recipient to an email sequence
- **create_reminder**: Create a new email reminder
- **get_availability**: Check user calendar availability
- **get_me**: Get current Mixmax user details
- **list_appointment_links**: List calendar scheduling links
- **list_contacts**: List Mixmax contacts
- **list_events**: List email analytics events
- **list_reminders**: List active email reminders
- **list_sequences**: List Mixmax email sequences
- **list_snippets**: List shared email snippets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mixmax** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email sequences."

**🤖 AI Agent:**
> Fetching sequences... I found 5 active sequences including 'New Lead Outreach' and 'Q4 Follow-up'.

---

**👤 You:**
> "Add john.doe@example.com to the 'Welcome' sequence."

**🤖 AI Agent:**
> Enrolling recipient... John Doe has been successfully added to the 'Welcome' sequence.

---

**👤 You:**
> "Check my recent email analytics."

**🤖 AI Agent:**
> Retrieving events... You had 12 opens and 3 link clicks in the last hour.


## ❓ FAQ

**Q: How do I find my Mixmax API Key?**
In Mixmax, go to Settings > Integrations > API to generate or copy your personal API token.

**Q: Can I add multiple recipients to a sequence at once?**
The current tool adds one recipient at a time for precision, but you can call it multiple times.

**Q: What kind of events are tracked?**
Mixmax tracks email opens, link clicks, attachment downloads, and replies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mixmax](https://vinkius.com/mcp/mixmax)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mixmax** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mixmax` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mixmax** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mixmax": {
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
