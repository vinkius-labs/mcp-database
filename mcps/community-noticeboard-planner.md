# Community Noticeboard Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-noticeboard-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Organize, validate, and schedule community announcements across multiple channels.

## Description
This MCP server provides a complete management system for community communications. It allows users to propose announcements, validate them against privacy and channel rules using `validate_announcement`, and generate optimized content for different mediums with `create_message_variants`. It also handles scheduling via `generate_posting_calendar` and manages ownership and removal tasks through `assign_ownership_and_reminders`.


## Available Tools (4)
- **create_message_variants**: Adapts a single announcement into different versions optimized for specific channels
- **generate_posting_calendar**: Creates a chronological schedule of all approved announcements
- **validate_announcement**: Checks if a single announcement proposal meets all systemic rules and privacy constraints
- **assign_ownership_and_reminders**: Maps announcements to owners and generates a list of upcoming removal tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Noticeboard Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Validate this announcement: 'Community meeting on Friday at 5pm' for 'Residents', via 'Digital Signage', from 2024-10-01 to 2024-10-05, contact 'admin@community.org', privacy 'public'."

**🤖 AI Agent:**
> The announcement is valid and approved for Digital Signage.

---

**👤 You:**
> "Create variants for 'Annual Summer Festival this Saturday!' for 'Email' and 'Digital Signage'."

**🤖 AI Agent:**
> Email: Join us for our Annual Summer Festival this Saturday! It will be a day of fun for everyone. Digital Signage: Annual Summer Festival! This Saturday.

---

**👤 You:**
> "Generate a posting calendar for an announcement active from 2024-12-01 to 2024-12-03 on 'Email'."

**🤖 AI Agent:**
> The schedule includes posts on 2024-12-01, 2024-12-02, and 2024-12-03 via Email.


## ❓ FAQ

**Q: How do I ensure my announcement follows privacy rules?**
You can use the `validate_announcement` tool, which automatically checks your content and privacy level against systemic constraints.

**Q: Can I get different versions of my message for social media and email?**
Yes, the `create_message_variants` tool adapts your original content into optimized versions for specific channels like Digital Signage or Email.

**Q: How are removal reminders handled?**
The `assign_ownership_and_reminders` tool automatically generates removal tasks for the day immediately following an announcement's end date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-noticeboard-planner](https://vinkius.com/en/ai-agent-connect/community-noticeboard-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Noticeboard Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-noticeboard-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Noticeboard Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-noticeboard-planner": {
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
