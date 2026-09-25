# Care Service Contract Review Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-service-contract-review-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze domestic care agreements against household priorities to identify risks and mismatches.

## Description
This MCP server provides specialized tools for families to evaluate domestic care service agreements. It identifies direct conflicts between contract terms and household priorities using `analyze_contract_alignment`. It evaluates financial and flexibility risks through `generate_risk_assessment`, verifies scheduling via `trace_schedule_feasibility`, and manages critical timelines with `track_decision_deadlines`. It helps uncover mismatches, negotiation points, and decision deadlines to ensure service continuity and alignment with family needs.


## Available Tools (4)
- **track_decision_deadlines**: Manage the timeline for making a final decision
- **analyze_contract_alignment**: Identify direct conflicts between the service contract and household priorities
- **generate_risk_assessment**: Evaluate danger posed by cancellation terms and financial structures
- **trace_schedule_feasibility**: Check if the proposed service schedule meets household availability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Service Contract Review Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare this contract with my priorities: priority is specialized nursing, but the contract only mentions general care."

**🤖 AI Agent:**
> A mismatch was identified: the household priority for specialized nursing is not covered by the general care terms in the contract.

---

**👤 You:**
> "Is the schedule feasible if I need care on Mondays from 8 AM to 4 PM and the provider is available Mondays from 10 AM to 2 PM?"

**🤖 AI Agent:**
> No, the schedule is not feasible. There is a conflict on Monday between 8 AM - 10 AM and 2 PM - 4 PM.

---

**👤 You:**
> "When is my decision deadline if the service starts on June 1st and requires 14 days notice?"

**🤖 AI Agent:**
> Your decision deadline is May 18th.


## ❓ FAQ

**Q: How does the tool identify mismatches?**
The `analyze_contract_alignment` tool compares the provided contract details against your stated household priorities to find discrepancies.

**Q: Can I check if the provider's schedule works for my family?**
Yes, you can use `trace_schedule_feasibility` to check if the proposed service schedule conflicts with your required availability.

**Q: How are financial risks evaluated?**
The `generate_risk_assessment` tool evaluates the danger posed by cancellation terms and specific rate structures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-service-contract-review-plan](https://vinkius.com/en/ai-agent-connect/care-service-contract-review-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Service Contract Review Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-service-contract-review-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Service Contract Review Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-service-contract-review-plan": {
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
