# Pet Overnight Care Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-overnight-care-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [scheduling](../categories/scheduling.md)

Orchestrate detailed overnight pet care plans with strict boundary enforcement.

## Description
This MCP server transforms pet owner requirements into actionable overnight care execution plans. It reconciles pet routines, provider availability, and strict care boundaries to ensure safety and consistency. Use `generate_care_plan` to create master arrangements, `validate_boundary_compliance` to audit sitter activities against owner constraints, `calculate_checkin_cadence` to schedule owner updates, and `resolve_contact_hierarchy` to organize emergency contact chains.


## Available Tools (4)
- **calculate_checkin_cadence**: Determines the optimal timing for updates based on owner preference and trip duration
- **generate_care_plan**: Creates the master execution plan by reconciling owner requests with provider availability
- **resolve_contact_hierarchy**: Organizes the emergency and backup contact chain
- **validate_boundary_compliance**: Audits a proposed set of care activities against the owner's strict limitations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Overnight Care Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a care plan for my dog from July 1st to July 5th. He needs feeding at 8am and 6pm, and a walk at 10am. The sitter is available all week. I allow extra treats but no off-leash walking."

**🤖 AI Agent:**
> The care plan for July 1st to July 5th is confirmed. The arrangement includes feeding at 8am and 6pm, and a 10am walk daily. Handoff notes include access instructions for the front door. Check-ins are scheduled daily via text.

---

**👤 You:**
> "Check if letting the dog run in the park without a leash is allowed based on my boundaries: { "permitted": ["extra treats"], "prohibited": ["off-leash walking"] }."

**🤖 AI Agent:**
> No, the activity 'running in the park without a leash' is a violation of the prohibited 'off-leash walking' constraint.

---

**👤 You:**
> "Calculate the check-in schedule for a 5-day trip with daily updates via text."

**🤖 AI Agent:**
> The check-in schedule for your 5-day trip includes one update per day via text, starting shortly after the initial handoff.


## ❓ FAQ

**Q: How does the system ensure pet safety?**
Safety is maintained by using `validate_boundary_compliance` to check all proposed activities against the owner's strict rules and `resolve_contact_hierarchy` to ensure a clear emergency contact chain.

**Q: Can I customize the update frequency?**
Yes, you can use `calculate_checkin_cadence` to determine the optimal timing for updates based on the duration of the care and your preferred communication method.

**Q: What happens if the sitter's availability doesn't match my dates?**
The `generate_care_plan` tool will identify if the requested absence dates are not a subset of the provider's availability and will return an error if they do not match.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-overnight-care-plan](https://vinkius.com/en/ai-agent-connect/pet-overnight-care-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Overnight Care Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-overnight-care-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Overnight Care Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-overnight-care-plan": {
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
