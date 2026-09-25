# Accessible Relocation Readiness Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-relocation-readiness-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Evaluates prospective residences against mandatory accessibility requirements and household needs.

## Description
This MCP server provides a decision-support engine for managing complex relocations. It evaluates prospective residences against non-negotiable mandatory access requirements, household equipment needs, and support arrangements. Use `evaluate_residence_viability` to determine if a property is a 'Move' or 'Decline', `generate_verification_plan` to identify missing data, `map_transition_responsibilities` to assign relocation tasks, and `create_first_week_setup_checklist` to ensure immediate accessibility upon arrival.


## Available Tools (4)
- **create_first_week_setup_checklist**: Generates a list of immediate physical setup actions required to ensure accessibility on day one
- **evaluate_residence_viability**: Determines if a specific residence is a "Move" or "Decline" based on the hierarchy of requirements
- **generate_verification_plan**: Identifies what information is still missing and creates a list of questions or actions needed to complete the evaluation
- **map_transition_responsibilities**: Breaks down the move from the current location to the new location into specific tasks assigned to specific parties


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Relocation Readiness Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Evaluate this residence: it has wide doorways and a roll-in shower, but I don't know if the hallway width is sufficient for my wheelchair."

**🤖 AI Agent:**
> The residence is currently classified as Tier 2 (Partially Accessible) because the hallway width is an unknown. Please use the verification plan to confirm the hallway dimensions.

---

**👤 You:**
> "I am moving on October 12th. I need to move a medical bed, a power wheelchair, and a specialized lift."

**🤖 AI Agent:**
> The transition plan has been generated. The Support Team is responsible for moving the medical bed and power wheelchair, while the Landlord must ensure the lift installation area is clear by October 11th.

---

**👤 You:**
> "What should I do on my first day in the new house with my new equipment?"

**🤖 AI Agent:**
> Your first-week setup includes: 1. Verifying power outlet availability for the medical bed (Critical), 2. Testing the roll-in shower drainage (Operational), and 3. Checking hallway clearance for the power wheelchair (Critical).


## ❓ FAQ

**Q: How does the tool decide if a residence is viable?**
The `evaluate_residence_viability` tool checks the residence against mandatory requirements first. If any mandatory requirement is missing, the residence is declined. If all are met, it scores the residence based on your specific preferences.

**Q: Can I use this to plan my actual moving day?**
Yes. You can use `map_transition_responsibilities` to break down tasks for the User, Support Team, and Landlord, and `create_first_week_setup_checklist` to prepare the new home for immediate use.

**Q: What happens if I don't have all the property details?**
If data is missing, the `generate_verification_plan` tool will identify the unknowns and provide a list of high-priority questions to ask the landlord or property manager.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-relocation-readiness-plan](https://vinkius.com/en/ai-agent-connect/accessible-relocation-readiness-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Relocation Readiness Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-relocation-readiness-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Relocation Readiness Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-relocation-readiness-plan": {
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
