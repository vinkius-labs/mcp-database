# Venture Down-Round Protection MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-down-round-protection)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Model the economic impact of anti-dilution provisions during venture down-rounds.

## Description
This MCP server provides specialized calculation engines to model the economic shifts caused by down-rounds in venture capital. It allows AI agents to determine how anti-dilution provisions, such as Full Ratchet or Weighted Average, affect equity ownership. Users can calculate investor protection value, founder dilution, and perform conversion analysis. The server also includes logic to handle pay-to-play provisions and simulate different anti-dilution scenarios to compare outcomes. Use `calculate_anti_dilution_impact` to find primary shifts, `apply_pay_to_play_logic` to adjust for participation, and `simulate_scenario_comparison` to evaluate different protection types.


## Available Tools (4)
- **apply_pay_to_play_logic**: Modify protection outcomes based on whether investors participate in the new round
- **calculate_anti_dilution_impact**: Determine the primary economic shifts in equity ownership caused by a down-round
- **get_conversion_summary**: Provide a high-level comparison of ownership before and after the down-round adjustment
- **simulate_scenario_comparison**: Compare the difference between a Full Ratchet and a Weighted Average outcome


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Down-Round Protection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the impact of a $2M investment at a $10M valuation when a down-round occurs at a $5M valuation using weighted average."

**🤖 AI Agent:**
> The weighted average adjustment results in an increased share count for the investor, providing specific protection value while increasing founder dilution to the calculated percentage.

---

**👤 You:**
> "Compare the protection value of Full Ratchet versus Weighted Average for a $1M investment with an original valuation of $20M and a down-round valuation of $10M."

**🤖 AI Agent:**
> The Full Ratchet provides significantly higher protection value compared to the Weighted Average approach for this specific scenario.

---

**👤 You:**
> "What happens to an investor's protection if they do not participate in the new round?"

**🤖 AI Agent:**
> If the investor does not participate, they lose their anti-dilution protections, which can be modeled using the pay-to-play logic tool.


## ❓ FAQ

**Q: What is the difference between Full Ratchet and Weighted Average?**
Full Ratchet is an aggressive protection that adjusts the conversion price to the new round's price. Weighted Average is a moderate approach that considers both the new price and the amount of capital raised. You can use `simulate_scenario_comparison` to see the difference in protection value between them.

**Q: How does pay-to-play affect my protection?**
If an investor does not participate in the new round, they may lose their anti-dilution rights. The `apply_pay_to_play_logic` tool can be used to calculate the resulting loss in protection.

**Q: Can I see the total dilution for founders?**
Yes. By using `calculate_anti_dilution_impact`, you can determine the specific percentage of equity lost by founders as a result of the anti-dilution adjustment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-down-round-protection](https://vinkius.com/en/ai-agent-connect/venture-down-round-protection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Down-Round Protection** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-down-round-protection` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Down-Round Protection** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-down-round-protection": {
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
