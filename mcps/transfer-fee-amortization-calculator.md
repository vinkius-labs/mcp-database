# Transfer Fee Amortization Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/transfer-fee-amortization-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate football player acquisition costs, amortization schedules, and impairment adjustments.

## Description
This MCP server provides precision financial tools for football clubs to manage player assets. It allows agents to calculate detailed amortization schedules, account for agent fees and registration costs, and manage contract changes. Use `get_amortization_schedule` to generate annual and monthly expense breakdowns, `get_impairment_adjustment` to handle value write-downs, `get_renewal_impact` for contract extensions, and `get_asset_summary` for a high-level financial snapshot of a player's book value.

### Available Tools

`amortization_schedule_tool`, `impairment_adjustment_tool`, `renewal_impact_tool`, `asset_summary_tool`


## Available Tools (4)
- **amortization_schedule_tool**: Generates a detailed breakdown of how the player's cost is recognized over time
- **asset_summary_tool**: Provides a high-level snapshot of the player's financial status
- **impairment_adjustment_tool**: g., injury) to adjust the book value.

Recalculates the remaining cost distribution after a player's value has been permanently reduced
- **renewal_impact_tool**: Calculates how extending a player's contract affects the future monthly cost of amortization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Transfer Fee Amortization Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the amortization for a player signed for 50,000,000 with a 5-year contract and 2,000,000 in agent fees."

**🤖 AI Agent:**
> The total acquisition cost is 52,000,000. Over a 60-month contract, the monthly expense is 866,666.67, with an annual expense of 10,400,000.

---

**👤 You:**
> "A player has a book value of 20,000,000. If we write down their value by 5,000,000 with 24 months remaining, what is the new monthly cost?"

**🤖 AI Agent:**
> The new book value is 15,000,000. With 24 months remaining, the new monthly expense is 625,000.

---

**👤 You:**
> "Give me a summary for a player with a 30,000,000 fee, 1,000,000 in agent fees, and 500,000 in registration costs, who has already been amortized by 10,000,000 over a 48-month contract."

**🤖 AI Agent:**
> The total acquisition cost is 31,500,000. The remaining book value is 21,500,000, with 10,000,000 already amortized and an original average monthly cost of 656,250.


## ❓ FAQ

**Q: How do I calculate the yearly expense for a new signing?**
You can use the `get_amortization_schedule` tool. Provide the transfer fee, contract duration, and any guaranteed add-ons or agent fees to receive a full breakdown of annual and monthly expenses. Tools available: `amortization_schedule_tool`, `impairment_adjustment_tool`, `renewal_impact_tool`.

**Q: What happens to the amortization if a player's value drops?**
When a player's value is reduced, use `get_impairment_adjustment`. This tool recalculates the remaining book value and provides a new monthly expense for the rest of the contract term.

**Q: Can I see the impact of extending a player's contract?**
Yes, the `get_renewal_impact` tool calculates how adding months to a contract affects the future monthly amortization expense based on the current book value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/transfer-fee-amortization-calculator](https://vinkius.com/en/ai-agent-connect/transfer-fee-amortization-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Transfer Fee Amortization Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `transfer-fee-amortization-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Transfer Fee Amortization Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "transfer-fee-amortization-calculator": {
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
