# Assistive Equipment Sharing Agreement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/assistive-equipment-sharing-agreement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Formalize logistical and legal frameworks for sharing assistive technology.

## Description
This MCP server provides a structured framework for managing the sharing of assistive technology. It allows owners to define rules for authorized users, manage reservation periods, and formalize handoff protocols. Use `generate_sharing_agreement` to create contracts, `get_handoff_checklist` to manage physical transfers, `resolve_usage_conflict` to handle disputes, and `generate_status_notification` to communicate equipment status.


## Available Tools (4)
- **generate_status_notification**: Produces the standardized messages sent to both parties regarding the movement and state of the equipment
- **get_handoff_checklist**: Provides the specific list of items and conditions that must be verified during the physical transfer of equipment
- **resolve_usage_conflict**: Orchestrates the formal steps to address disagreements between owner and user
- **generate_sharing_agreement**: Creates the formal contract between the owner and the user for a specific piece of equipment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Assistive Equipment Sharing Agreement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a sharing agreement for user 'user_123' to use equipment 'wheelchair_001' from 2024-06-01 to 2024-06-05 with owner 'owner_999'."

**🤖 AI Agent:**
> The sharing agreement has been successfully created. Agreement ID: AG-7782. Status: Active. Terms: User is authorized for the specified period under the owner's liability framework.

---

**👤 You:**
> "I need the checklist for the return of agreement 'AG-7782'."

**🤖 AI Agent:**
> The return checklist for AG-7782 includes: 1. Verify battery charge level. 2. Inspect frame for structural integrity. 3. Confirm all accessories are present. Location: Central Pickup Point.

---

**👤 You:**
> "The user returned the equipment late for agreement 'AG-7782'. How do I resolve this?"

**🤖 AI Agent:**
> To resolve the late return, use the `resolve_usage_conflict` tool with the conflict type 'late_return' and provide the details of the delay.


## ❓ FAQ

**Q: How do I create a contract for a new equipment loan?**
You can use the `generate_sharing_agreement` tool by providing the owner ID, user ID, equipment ID, and the requested reservation period.

**Q: What happens if there is a disagreement about the equipment condition?**
Disagreements can be addressed using the `resolve_usage_conflict` tool, which follows the pre-agreed liability rules and conflict-resolution process.

**Q: How can I verify the equipment state during pickup or return?**
Use the `get_handoff_checklist` tool to retrieve the specific items and condition expectations required for the transfer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/assistive-equipment-sharing-agreement](https://vinkius.com/en/ai-agent-connect/assistive-equipment-sharing-agreement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Assistive Equipment Sharing Agreement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `assistive-equipment-sharing-agreement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Assistive Equipment Sharing Agreement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "assistive-equipment-sharing-agreement": {
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
