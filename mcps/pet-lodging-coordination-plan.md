# Pet Lodging Coordination Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-lodging-coordination-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Coordinates pet stay compatibility and generates compliance checklists for lodging.

## Description
This MCP connects AI agents to a coordination engine that evaluates if a pet profile matches specific lodging rules. It uses `evaluate_stay_compatibility` to determine if a stay is possible, `generate_arrival_checklist` for check-in preparation, `get_in_stay_responsibilities` to outline owner obligations, and `generate_checkout_actions` to ensure property compliance upon departure.


## Available Tools (4)
- **evaluate_stay_compatibility**: Determines if a proposed lodging is viable for a specific pet and stay configuration
- **generate_arrival_checklist**: Provides a list of tasks the user must complete to ensure a smooth check-in
- **generate_checkout_actions**: Provides instructions for leaving the property to ensure compliance
- **get_in_stay_responsibilities**: Outlines the behavioral and logistical obligations of the pet owner during the stay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Lodging Coordination Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can my 50lb Golden Retriever stay at lodging ID 'hotel_123' from June 1st to June 5th?"

**🤖 AI Agent:**
> Yes, the stay is possible. The Golden Retriever meets the weight and breed requirements for hotel_123.

---

**👤 You:**
> "What are my responsibilities while staying at 'resort_abc' with my pet?"

**🤖 AI Agent:**
> Your responsibilities include keeping your pet on a leash at all times and disposing of all pet waste in designated bins.

---

**👤 You:**
> "Give me a checkout checklist for 'cabin_456' using a deluxe room."

**🤖 AI Agent:**
> Please ensure all pet hair is vacuumed from the rug and any pet-related odors are neutralized before departing.


## ❓ FAQ

**Q: How do I know if my pet can stay at a specific hotel?**
You can use the `evaluate_stay_compatibility` tool to check if your pet's species, breed, and weight meet the property's specific rules.

**Q: Does this tool provide checkout instructions?**
Yes, the `generate_checkout_actions` tool provides specific instructions to ensure you follow property policies and avoid extra fees.

**Q: Can I get a checklist for my arrival?**
Yes, the `generate_arrival_checklist` tool creates a task list based on your arrival method and your pet's needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-lodging-coordination-plan](https://vinkius.com/en/ai-agent-connect/pet-lodging-coordination-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Lodging Coordination Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-lodging-coordination-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Lodging Coordination Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-lodging-coordination-plan": {
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
