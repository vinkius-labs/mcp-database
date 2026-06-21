# Indemnification Exposure Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/indemnification-exposure-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate maximum financial exposure in indemnity clauses by assessing contractual caps, carve-outs, and jurisdiction.

## Description
This MCP server provides tools to quantify the potential financial risks associated with indemnification clauses in legal contracts. By analyzing the interaction between contractual caps, specific carve-outs (such as IP infringement or fraud), and jurisdictional legal standards, agents can determine the worst-case exposure scenario. Use `calculate_standard_cap` to find the primary liability ceiling, `evaluate_carveout_impact` to estimate additional risk from exceptions, and `calculate_worst_case_exposure` for a comprehensive breakdown of total potential loss.


## Available Tools
- **evaluate_carveout_impact**: Estimates the additional liability exposure introduced by specific carve-out events
- **calculate_standard_cap**: Calculates the maximum dollar amount allowed under the standard cap
- **calculate_worst_case_exposure**: Aggregates standard caps, carve-outs, and damage type considerations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Indemnification Exposure Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the standard cap for a $500,000 contract with a 2x multiplier."

**🤖 AI Agent:**
> The calculated standard cap is $1,000,000.

---

**👤 You:**
> "What is the worst-case exposure for a $1M contract with a 1x cap and active IP_INFRINGEMENT carve-out?"

**🤖 AI Agent:**
> The total worst-case exposure is $2,000,000 ($1,000,000 standard cap + $1,000,000 from the carve-out).

---

**👤 You:**
> "Estimate the impact of fraud and gross negligence on a $250,000 contract."

**🤖 AI Agent:**
> The additional exposure from these two carve-outs is estimated at $500,000.


## ❓ FAQ

**Q: How can I calculate the primary liability limit?**
You can use the `calculate_standard_cap` tool by providing the total contract value and the multiplier applied to it.

**Q: What happens when a carve-out is active?**
When using `evaluate_carveout_impact`, the tool estimates that each active event, such as fraud or IP infringement, adds exposure equal to the base contract value.

**Q: Can I see a full breakdown of all potential losses?**
Yes. The `calculate_worst_case_exposure` tool provides a detailed breakdown including standard caps, carve-outs, and the impact of different damage types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/indemnification-exposure-calculator](https://vinkius.com/mcp/indemnification-exposure-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Indemnification Exposure Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `indemnification-exposure-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Indemnification Exposure Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "indemnification-exposure-calculator": {
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
