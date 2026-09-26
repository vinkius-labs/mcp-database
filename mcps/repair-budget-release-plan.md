# Repair Budget & Release Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-budget-release-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Synchronize project budgets with verifiable milestone completion and gated payments.

## Description
This MCP server provides financial control tools to manage project cash flow through gated payments and milestone verification. It allows users to generate payment schedules, calculate holdbacks, and verify if specific milestone gates are cleared using `verify_milestone_gate`. You can also monitor reserve funds with `track_contingency_usage` and retrieve inspection requirements via `get_approval_checklist`. It acts as a bridge between project planning and financial execution, ensuring funds are only released when the required evidence is provided.


## Available Tools (5)
- **calculate_holdbacks**: 
- **generate_payment_schedule**: 
- **get_approval_checklist**: 
- **track_contingency_usage**: 
- **verify_milestone_gate**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair Budget & Release Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a payment schedule for a $50,000 project with a $5,000 deposit and two milestones: Foundation ($20,000) and Framing ($20,000)."

**🤖 AI Agent:**
> The payment schedule includes a $5,000 deposit at commencement, followed by $20,000 for the Foundation milestone and $20,000 for the Framing milestone, totaling $45,000 in milestone payments.

---

**👤 You:**
> "Check if the milestone 'Roofing' is cleared with the following evidence: 'Site Photo', 'Signed Invoice'. The required evidence is 'Site Photo' and 'Signed Invoice'."

**🤖 AI Agent:**
> The gate is Open. All required evidence has been verified.

---

**👤 You:**
> "What is the inspection checklist for the 'Electrical' milestone?"

**🤖 AI Agent:**
> The inspection items for the Electrical milestone are: Wiring integrity check, Grounding verification, and Panel labeling.


## ❓ FAQ

**Q: How do I ensure payments are only made after work is verified?**
You can use the `verify_milestone_gate` tool to check if the provided evidence matches the required documentation or inspection results before releasing funds.

**Q: Can I track my emergency funds?**
Yes, the `track_contingency_usage` tool monitors your reserve fund and provides a status of whether your contingency is healthy, at warning, or exhausted.

**Q: How are holdbacks calculated?**
The `calculate_holdbacks` tool calculates the specific amount to be withheld from each milestone based on a fixed percentage you define.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-budget-release-plan](https://vinkius.com/en/ai-agent-connect/repair-budget-release-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair Budget & Release Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-budget-release-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair Budget & Release Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-budget-release-plan": {
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
