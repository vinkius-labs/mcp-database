# Emergency Information Board Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/emergency-information-board-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate printable emergency boards and privacy-focused separation plans.

## Description
This MCP server helps households prepare for emergencies by organizing critical information. It uses the Least-Sensitive-Display Rule to ensure privacy by separating public utility data from sensitive details. Use `list_printable_board` to create a physical layout for your fridge or command center, `generate_separation_plan` to split data between public and private layers, `create_explanation_script` to communicate rules to your household, and `schedule_refresh_reminder` to track when your information needs updating.


## Available Tools (4)
- **create_explanation_script**: Provides a verbal script to help a user explain the emergency plan to their household
- **generate_separation_plan**: Creates a plan to divide information between the public board and a private folder
- **list_printable_board**: Generates a structured layout for a physical emergency board
- **schedule_refresh_reminder**: Calculates and provides instructions for when the user needs to update their information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Information Board Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a printable board layout for my fridge with these contacts: John (Neighbor), Sarah (Emergency Services), and meeting place: Oak Park."

**🤖 AI Agent:**
> EMERGENCY BOARD
Location: Kitchen Fridge

CONTACTS:
- Neighbor: John
- Emergency Services: Sarah

MEETING PLACE:
- Oak Park

Last Verified: 2023-10-27

---

**👤 You:**
> "Help me explain the privacy rules to my roommates."

**🤖 AI Agent:**
> Hey everyone, I've set up an emergency board. To keep our private info safe from visitors, we're only putting basic info like meeting spots on the fridge. Detailed stuff like medical info will stay in our private folder.

---

**👤 You:**
> "When is my next update due if I last updated on 2023-01-01 and want to update every 90 days?"

**🤖 AI Agent:**
> Your next update is due on 2023-04-01. Status: OVERDUE.


## ❓ FAQ

**Q: How does this tool protect my privacy?**
It applies the Least-Sensitive-Display Rule, which ensures that sensitive information is moved to a private dossier while only non-identifiable data is placed on the public board.

**Q: What is a printable board layout?**
It is a structured visual arrangement of contact, location, and logistics data designed to be printed and posted in a visible household area.

**Q: How often should I update my emergency plan?**
You can use `schedule_refresh_reminder` to calculate your next update date based on your preferred refresh interval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/emergency-information-board-plan](https://vinkius.com/en/ai-agent-connect/emergency-information-board-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Information Board Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-information-board-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Information Board Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-information-board-plan": {
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
