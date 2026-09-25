# Care Laundry Household Rotation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-laundry-household-rotation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Manages laundry task rotation, storage capacity, and helper availability.

## Description
This MCP server manages the complex logistics of household laundry. It uses `schedule_laundry_rotation` to distribute tasks among available helpers while respecting storage limits. It also provides logistical support through `get_pickup_instructions`, manages service continuity with `calculate_fallback_plan`, and ensures privacy-compliant transitions using `generate_handoff_list`.


## Available Tools (4)
- **calculate_fallback_plan**: Determines the next steps when the primary rotation fails to find an available helper
- **generate_handoff_list**: Creates a clean, privacy-compliant summary for the household transition
- **get_pickup_instructions**: Generates specific logistical instructions for the assigned helper
- **schedule_laundry_rotation**: Calculates the optimal distribution of laundry tasks among available helpers while respecting all constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Laundry Household Rotation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Schedule laundry for Monday and Wednesday with a storage limit of 5 units."

**🤖 AI Agent:**
> Laundry tasks have been scheduled for Monday and Wednesday. Total capacity used is within the 5-unit limit.

---

**👤 You:**
> "Generate pickup instructions for the laundry located in the basement."

**🤖 AI Agent:**
> Please collect the laundry from the basement using the standard pickup method.

---

**👤 You:**
> "Create a handoff list for the helper with minimal privacy masking."

**🤖 AI Agent:**
> Handoff complete: 3 tasks assigned at the laundry room location.


## ❓ FAQ

**Q: How does the rotation work?**
The system uses `schedule_laundry_rotation` to match laundry tasks with helpers based on their specific availability days and the household's storage capacity.

**Q: What happens if no helper is available?**
If a task cannot be assigned, the `calculate_fallback_plan` tool determines the next step based on your chosen policy, such as notifying the user.

**Q: Is helper information kept private?**
Yes. The `generate_handoff_list` tool applies privacy rules to mask personal details during household transitions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-laundry-household-rotation](https://vinkius.com/en/ai-agent-connect/care-laundry-household-rotation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Laundry Household Rotation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-laundry-household-rotation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Laundry Household Rotation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-laundry-household-rotation": {
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
