# Repair Contingency Response Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-contingency-response-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Automated risk assessment and contingency planning for repair projects.

## Description
This MCP server provides a specialized engine for managing repair project risks. It allows AI agents to evaluate risk severity using `evaluate_risk_status`, calculate the depletion of budget and schedule buffers with `calculate_resource_impact`, and generate actionable response plans via `generate_contingency_plan`. Additionally, it provides ready-to-use stakeholder notification templates through `get_communication_scripts` to ensure clear communication during contingency activation.


## Available Tools (4)
- **calculate_resource_impact**: Determine budget and schedule consumption by risks
- **evaluate_risk_status**: Determine if project risks have crossed thresholds requiring contingency activation
- **generate_contingency_plan**: Produce actions, approvals, and vendor switches
- **get_communication_scripts**: Provide text templates for stakeholder notification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Contingency Response Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if our current risks have crossed the critical threshold."

**🤖 AI Agent:**
> The current risk score of 85 exceeds the critical threshold of 80, requiring immediate executive intervention.

---

**👤 You:**
> "How much budget reserve will be left if the electrical repair costs $5,000?"

**🤖 AI Agent:**
> After the $5,000 repair cost, the remaining budget reserve is $15,000.

---

**👤 You:**
> "Generate a communication script for an executive regarding a budget allocation."

**🤖 AI Agent:**
> Subject: Urgent: Contingency Budget Allocation Required. Dear Executive, a critical risk has triggered a budget allocation of $5,000 to address electrical repairs.


## ❓ FAQ

**Q: How does the system determine if a risk requires action?**
The system uses `evaluate_risk_status` to compare calculated risk scores against pre-defined warning and critical thresholds.

**Q: Can I calculate how much budget is left after a risk occurs?**
Yes, the `calculate_resource_impact` tool calculates the remaining budget and schedule slack based on the estimated impact of realized risks.

**Q: What happens if a primary vendor fails?**
You can use `generate_contingency_plan` to identify suitable alternate vendors from the pre-approved vendor catalog.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-contingency-response-plan](https://vinkius.com/en/ai-agent-connect/repair-contingency-response-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Contingency Response Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-contingency-response-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Contingency Response Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-contingency-response-plan": {
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
