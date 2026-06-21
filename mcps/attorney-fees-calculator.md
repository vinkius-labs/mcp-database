# Attorney Fees Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/attorney-fees-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate and compare legal billing models including hourly, contingency, flat fee, and blended rates.

## Description
The Attorney Fees Calculator MCP server provides precise financial projections for various legal billing structures. Use `getHourlyEstimate` to determine costs based on attorney seniority, or `getContingencyEstimate` to calculate attorney shares and client net recovery across different litigation stages like pre-suit or post-appeal. The server also supports `getFlatFeeQuote` for fixed contract prices and `getBlendedTeamCost` for complex team assignments. For strategic decision-making, use `analyzeFeeBreakEven` to find the exact recovery threshold where contingency fees align with hourly costs.

### Available Tools

`hourly.estimate`, `contingency.estimate`, `flat_fee.quote`, `team.cost`, `fee.break_even`


## Available Tools (5)
- **contingency**: Calculates the attorney's share and the client's net recovery
- **flat_fee**: Retrieves a fixed price for specific legal contract types
- **hourly**: Calculates the total cost for a single attorney based on time and seniority
- **fee**: Compares different billing structures to find the threshold
- **team**: Calculates the total cost for a legal team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Attorney Fees Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost for a junior attorney working 10 hours."

**🤖 AI Agent:**
> The `getHourlyEstimate` tool would return the total fee based on the standard junior rate multiplied by 10 hours.

---

**👤 You:**
> "What is my client's net recovery if we win $100,000 in the post-filing stage?"

**🤖 AI Agent:**
> Using `getContingencyEstimate` with a recovery amount of 100000 and stage 'post_filing', the tool will calculate the attorney's percentage and show the remaining net amount for the client.

---

**👤 You:**
> "Find the break-even point between a $50,000 contingency win and an hourly model with 50 hours of partner time."

**🤖 AI Agent:**
> The `analyzeFeeBreakEven` tool will process the expected recovery and planned hours to identify the specific gross recovery amount where both models cost the same.


## ❓ FAQ

**Q: How do I calculate costs for a team of lawyers?**
Use the `getBlendedTeamCost` tool by providing a JSON array of assignments, where each object contains the hours worked and the seniority level for each team member. Tools available: `hourly.estimate`, `contingency.estimate`, `flat_fee.quote`.

**Q: Can I compare contingency fees against hourly rates?**
Yes, the `analyzeFeeBreakEven` tool is specifically designed to find the recovery amount threshold where different billing models intersect.

**Q: What litigation stages are supported for contingency calculations?**
The tool supports `pre_suit`, `post_filing`, and `post_appeal` stages, with the percentage fee scaling according to the complexity of each stage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/attorney-fees-calculator](https://vinkius.com/mcp/attorney-fees-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Attorney Fees Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `attorney-fees-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Attorney Fees Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "attorney-fees-calculator": {
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
