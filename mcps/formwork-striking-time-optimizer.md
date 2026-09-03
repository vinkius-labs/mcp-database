# Formwork Striking Time Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/formwork-striking-time-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates safe formwork removal timing based on concrete strength and environmental factors.

## Description
This MCP server provides critical engineering calculations for structural concrete management. It connects AI agents to specialized tools for determining the minimum number of days required before formwork can be safely removed using `calculate_striking_time`. It also provides logical support removal sequences via `get_reshoring_sequence`, performs safety audits with `perform_safety_audit`, and evaluates structural weight movement using `analyze_load_transfer`. This ensures structural integrity during the transition from formwork to self-supporting concrete.

### Available Tools

`calculate_striking_time_tool`, `get_reshoring_sequence_tool`, `perform_safety_audit_tool`, `analyze_load_transfer_tool`


## Available Tools (4)
- **analyze_load_transfer_tool**: Evaluates how the weight of the structure will move from the formwork to the concrete
- **calculate_striking_time_tool**: Determines the minimum number of days required before formwork can be safely removed
- **perform_safety_audit_tool**: Validates if the current stripping plan meets all engineering safety constraints
- **get_reshoring_sequence_tool**: Provides a logical order for the removal of temporary supports (props) to prevent overloading


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formwork Striking Time Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When can I safely remove the formwork for a slab that needs 80% strength, currently at 15 MPa, at 22 degrees Celsius using moist curing?"

**🤖 AI Agent:**
> The minimum stripping time is 5 days, with an estimated strength of 22.4 MPa at the time of removal.

---

**👤 You:**
> "Give me the removal order for 10 props on a beam on day 4 of curing."

**🤖 AI Agent:**
> The removal order is: remove props 1-3, then 4-6, then 7-8. 2 props must remain in place.

---

**👤 You:**
> "Is it safe to strip a column with 25 MPa strength if the design strength is 30 MPa and reshoring is active?"

**🤖 AI Agent:**
> No, the stripping plan does not meet safety standards. Violation: current strength is below the critical threshold for this element type. Recommended action: Hold stripping.


## ❓ FAQ

**Q: How does temperature affect the stripping time?**
Higher temperatures accelerate the chemical hydration process, which reduces the number of days required before the concrete reaches the necessary strength for safe removal. Tools available: `calculate_striking_time_tool`, `get_reshoring_sequence_tool`, `perform_safety_audit_tool`.

**Q: Can I use this to manage my props?**
Yes, you can use the `get_reshoring_sequence` tool to receive a step-by-step list of which props to remove to prevent overloading the structure.

**Q: What happens if the safety audit fails?**
If `perform_safety_audit` returns a failure, it will provide specific violations and a recommended action, such as holding the stripping process or resuming curing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/formwork-striking-time-optimizer](https://vinkius.com/ai-agent-connect/formwork-striking-time-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formwork Striking Time Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formwork-striking-time-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formwork Striking Time Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formwork-striking-time-optimizer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
