# Relative Contact Change Log MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/relative-contact-change-log)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and manage contact information updates for family members with scheduled effective dates.

## Description
This MCP server provides a specialized system for managing contact information changes for relatives. It allows users to log modifications, schedule them for future effective dates, and generate organized checklists to ensure all necessary notification recipients are informed. Use `log_contact_change` to record new updates, `get_relative_contact_details` to view current information, `get_update_checklist` to see upcoming tasks, and `mark_change_complete` to finalize a change once notifications are sent.


## Available Tools (4)
- **get_relative_contact_details**: Retrieves the current, active contact information for a specific relative
- **get_update_checklist**: Generates a prioritized list of tasks that need to be completed based on upcoming contact changes
- **log_contact_change**: The effective date must be today or in the future.

Records a new modification to a relative's contact information
- **mark_change_complete**: Finalizes a change entry after the notifications have been sent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relative Contact Change Log** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Log a change for relative ID 'rel-123' changing their email and phone, effective next Monday."

**🤖 AI Agent:**
> The change for relative rel-123 has been logged with an effective date of 2025-05-19.

---

**👤 You:**
> "What are the current contact details for relative 'rel-456'?"

**🤖 AI Agent:**
> The current contact details for rel-456 are: Email: jane.doe@example.com, Phone: 555-0123, Address: 123 Maple St.

---

**👤 You:**
> "Show me my update checklist for the next two weeks."

**🤖 AI Agent:**
> You have 2 pending changes: 1. Relative rel-789 (Email) effective 2025-05-20. 2. Relative rel-012 (Address) effective 2025-05-25.


## ❓ FAQ

**Q: How do I record a new contact change?**
You can use the `log_contact_change` tool to record a modification, specifying the relative ID, the fields being changed, the effective date, and the people who need to be notified.

**Q: Can I schedule a change for a future date?**
Yes, when using `log_contact_change`, you can provide an effective date in the future. The change will remain pending until that date is reached.

**Q: How do I know which notifications I still need to send?**
Use the `get_update_checklist` tool to generate a prioritized list of pending changes organized by their effective date.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/relative-contact-change-log](https://vinkius.com/en/ai-agent-connect/relative-contact-change-log)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relative Contact Change Log** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relative-contact-change-log` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relative Contact Change Log** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relative-contact-change-log": {
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
