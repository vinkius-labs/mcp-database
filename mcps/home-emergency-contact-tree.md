# Home Emergency Contact Tree MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-emergency-contact-tree)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize household members and external contacts into a prioritized, rule-based emergency call tree.

## Description
Manage crisis response with a structured communication system. This MCP allows AI agents to generate prioritized notification sequences using `get_notification_plan`, produce printable `generate_contact_cards`, retrieve tailored `get_message_templates`, and manage data accuracy with `get_maintenance_tasks`.


## Available Tools (4)
- **generate_contact_cards**: Produces formatted, printable information for quick reference during a crisis
- **get_maintenance_tasks**: Provides a list of required administrative actions to ensure the contact tree remains accurate
- **get_message_templates**: Retrieves pre-written message text tailored to the contact type and emergency severity
- **get_notification_plan**: Generates a step-by-step sequence of who to contact and how to reach them based on an emergency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Emergency Contact Tree** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a notification plan for household members 123 and 456 during a critical emergency."

**🤖 AI Agent:**
> The notification sequence for a critical emergency is: 1. Member 123 (SMS), 2. Member 456 (Voice Call), 3. Nearby Contact (SMS).

---

**👤 You:**
> "Generate printable contact cards for my nearby contacts."

**🤖 AI Agent:**
> Here are your nearby contact cards: John Doe (555-0101), Jane Smith (555-0102).

---

**👤 You:**
> "What message should I send to a neighbor for a minor emergency?"

**🤖 AI Agent:**
> A suitable SMS template is: 'Hello, this is an update regarding a minor household matter. Please let us know when you are available.'


## ❓ FAQ

**Q: How does the notification order work?**
The system follows a strict hierarchy: it first attempts to contact household members, then moves to nearby contacts, and finally reaches out to out-of-area contacts if needed.

**Q: Can I print contact information for physical use?**
Yes, you can use the tool to generate formatted, printable contact cards for any group, such as household or nearby contacts.

**Q: How often should I update my contact information?**
It is recommended to verify your contact tree every 90 days to ensure all phone numbers and relationships remain accurate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-emergency-contact-tree](https://vinkius.com/en/ai-agent-connect/home-emergency-contact-tree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Emergency Contact Tree** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-emergency-contact-tree` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Emergency Contact Tree** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-emergency-contact-tree": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
