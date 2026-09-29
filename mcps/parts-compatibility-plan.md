# Parts Compatibility Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/parts-compatibility-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Validate part compatibility and generate purchase and installation plans.

## Description
This MCP server provides a precision matching engine for industrial components. It allows AI agents to validate if a candidate part meets manufacturer specifications and user constraints. Use `get_compatibility_report` to check specific parts, `generate_purchase_plan` to source compatible components within a budget, `get_installation_requirements` for logistical preparation, and `validate_part_constraints` to ensure user requirements are physically feasible.


## Available Tools (4)
- **get_compatibility_report**: Determine if a specific candidate part is suitable for a target model under given user constraints
- **get_installation_requirements**: Provide the necessary physical and logistical steps required to install a matched part
- **validate_part_constraints**: Check if a set of user constraints is logically sound and possible within the context of a specific model
- **generate_purchase_plan**: Create a list of all compatible parts that can be acquired to complete a specific project requirement


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parts Compatibility Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is part P-100 compatible with model M-500 given a max price of 500?"

**🤖 AI Agent:**
> The part P-100 is compatible with model M-500 and falls within your budget.

---

**👤 You:**
> "Generate a purchase plan for model M-200 with a budget of 1000."

**🤖 AI Agent:**
> The total estimated cost for compatible parts is 850, which is within your budget.

---

**👤 You:**
> "What tools do I need to install part P-202 on model M-101?"

**🤖 AI Agent:**
> You will need a torque wrench and a specialized alignment jig for this installation.


## ❓ FAQ

**Q: How does the compatibility check work?**
The system checks if the candidate part's attributes fall within the allowed ranges defined in the Manufacturer Specifications and satisfy all provided user constraints.

**Q: Can I generate a full procurement list?**
Yes, you can use the `generate_purchase_plan` tool to identify all compatible parts that fit your target model and budget.

**Q: What information is needed for installation prep?**
You need the `modelId` and the `partId` to retrieve required tools, safety protocols, and estimated duration via `get_installation_requirements`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/parts-compatibility-plan](https://vinkius.com/en/ai-agent-connect/parts-compatibility-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Parts Compatibility Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `parts-compatibility-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Parts Compatibility Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "parts-compatibility-plan": {
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
