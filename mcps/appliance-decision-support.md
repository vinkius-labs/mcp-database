# Appliance Decision Support MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/appliance-decision-support)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Evaluate whether to repair or replace household appliances.

## Description
This MCP server provides a decision-support engine for household appliance management. It helps users determine if they should repair an existing unit or invest in a replacement by analyzing age, symptoms, warranty status, and repair costs. Use `get_decision_brief` to receive a full recommendation, `get_service_booking_requirements` to prepare for a technician, `get_replacement_transition_checklist` for moving to a new unit, and `get_economic_lifespan_analysis` to assess long-term financial health.


## Available Tools (4)
- **get_economic_lifespan_analysis**: Evaluate remaining value and replacement urgency
- **get_decision_brief**: Evaluate whether to repair or replace an appliance
- **get_replacement_transition_checklist**: Provide a logistical roadmap for replacing an appliance
- **get_service_booking_requirements**: Generate necessary details for scheduling a professional repair


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Appliance Decision Support** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My refrigerator is 6 years old, the compressor is making a loud noise, it is not under warranty, the repair quote is $300, and a new one costs $1200. My repair threshold is 25%. Should I repair or replace?"

**🤖 AI Agent:**
> REPAIR. The repair cost of $300 is 25% of the $1200 replacement cost, which meets your threshold. Since the appliance is mid-life, repairing is the recommended path.

---

**👤 You:**
> "I need to replace my washing machine. It's a front-loader, I need to know if I need special installation and how to get rid of the old one."

**🤖 AI Agent:**
> To replace your washing machine, you should first verify that the new unit's water inlet and electrical connections match your current setup. You should also schedule a professional removal service to handle the disposal of the old unit.

---

**👤 You:**
> "Is my 10-year-old dishwasher still worth fixing?"

**🤖 AI Agent:**
> Given the age of 10 years, the appliance is likely at its end-of-life. Even if a repair is relatively inexpensive, the high probability of future failures suggests that replacement is the more stable long-term decision.


## ❓ FAQ

**Q: How does the tool decide between repair and replacement?**
The decision is based on comparing the `currentServiceQuote` against a user-defined `repairThreshold` percentage of the `replacementCost`, while also considering the appliance age and warranty status.

**Q: Can I use this to prepare for a repair technician?**
Yes, by using `get_service_booking_requirements`, you can generate a list of necessary information like serial numbers and technical notes to provide to the professional.

**Q: What happens if my appliance is under warranty?**
If `warrantyStatus` is true, the engine prioritizes repair if the symptom is a covered defect, as this minimizes out-of-pocket costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/appliance-decision-support](https://vinkius.com/en/ai-agent-connect/appliance-decision-support)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Appliance Decision Support** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `appliance-decision-support` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Appliance Decision Support** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "appliance-decision-support": {
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
