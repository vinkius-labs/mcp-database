# Pet Trip Care Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-trip-care-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Generates comprehensive pet care execution plans by matching trip dates and pet constraints with available care options.

## Description
This MCP server provides a structured decision-support system for pet owners planning travel. It evaluates care options--such as sitters, boarding facilities, or family--against non-negotiable pet constraints like social needs or mobility limits. Using tools like `find_optimal_care_location`, it identifies the best fit, then uses `generate_execution_actions` to create booking and handoff steps. It also uses `plan_communication_and_backup` to establish update schedules and `create_return_transition` to manage the pet's return and final payment.


## Available Tools (4)
- **create_return_transition**: Outlines the logistics for the end of the care period
- **find_optimal_care_location**: Determines the best location for pet care by applying non-negotiable constraints first
- **generate_execution_actions**: Creates the logistical steps for booking the care and managing the pet's handoff
- **plan_communication_and_backup**: Establishes how the owner will stay informed and provides a safety net


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Trip Care Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm traveling from June 1st to June 10th. My dog needs a sitter because he can't be around other dogs. I have a sitter available for $50/day and a kennel for $40/day. Which is better?"

**🤖 AI Agent:**
> The best location is the Home-Sitter. Since your dog cannot be around other dogs, the communal kennel is disqualified. The sitter is the only valid option that meets your pet's social constraints.

---

**👤 You:**
> "Help me plan the handoff for my pet sitter."

**🤖 AI Agent:**
> To complete the handoff, you should confirm the sitter's arrival time, drop off the pet's food and medication, and ensure the leash and carrier are ready for transport.

---

**👤 You:**
> "What should I do when I get back from my trip on July 15th?"

**🤖 AI Agent:**
> Upon your return on July 15th, you should meet the caregiver at the agreed location to pick up your pet and then process the final payment of the agreed amount.


## ❓ FAQ

**Q: How does the tool decide on a care location?**
The `find_optimal_care_location` tool first filters all available options against your pet's non-negotiable constraints. Only options that meet these safety and physical needs are considered before selecting the best one based on your preferences.

**Q: Can I get a backup plan if my primary sitter cancels?**
Yes. The `plan_communication_and_backup` tool identifies a secondary, pre-vetted option from your list of available options that satisfies your pet's constraints.

**Q: Does this tool provide medical advice for my pet?**
No. This system is strictly for logistical planning and care coordination. It does not provide veterinary or medical advice.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-trip-care-planner](https://vinkius.com/en/ai-agent-connect/pet-trip-care-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Trip Care Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-trip-care-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Trip Care Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-trip-care-planner": {
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
