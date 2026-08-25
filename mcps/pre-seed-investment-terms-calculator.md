# Pre-Seed Investment Terms Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pre-seed-investment-terms-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Model early-stage investment structures like SAFE and Convertible Notes.

## Description
This MCP server provides specialized tools for modeling early-stage investment structures. It allows AI agents to calculate effective valuations, equity percentages, and dilution scenarios for SAFE and Convertible Note investments. Use `calculate_conversion_outcome` to determine the primary conversion metrics, `compare_cap_vs_discount` to analyze the trade-off between valuation caps and discount rates, or `simulate_dilution_scenarios` to project ownership across various future company valuations.


## Available Tools (3)
- **calculate_conversion_outcome**: Determines primary conversion metrics for an investment instrument
- **compare_cap_vs_discount**: Analyzes the trade-off between the Valuation Cap and the Discount Rate
- **simulate_dilution_scenarios**: Projects ownership under different future valuation scenarios


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pre-Seed Investment Terms Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the conversion outcome for a $500,000 SAFE with a $5M valuation cap and a 20% discount, assuming the next round valuation is $10M."

**🤖 AI Agent:**
> The effective valuation is $5,000,000, resulting in an equity percentage of 10.0%.

---

**👤 You:**
> "Compare the cap vs discount for a $250,000 investment with a $4M cap and a 15% discount when the next round is $6M."

**🤖 AI Agent:**
> The Valuation Cap is the primary driver, providing more value to the investor than the Discount Rate.

---

**👤 You:**
> "What happens to a $100,000 Note with 5% interest and a $3M cap if the next round is $5M?"

**🤖 AI Agent:**
> The total investment value including interest is $105,000, and the effective valuation is $3,000,000, resulting in 3.5% equity.


## ❓ FAQ

**Q: What is the difference between a SAFE and a Convertible Note?**
A SAFE is a contract for future equity without interest, while a Convertible Note is a debt instrument that accumulates interest before converting into equity.

**Q: How does the valuation cap affect my equity?**
The valuation cap sets a maximum price for conversion, ensuring you receive a specific minimum equity percentage if the next round's valuation is significantly higher.

**Q: Can I simulate different exit valuations?**
Yes, you can use the `simulate_dilution_scenarios` tool to project ownership percentages across a range of potential future company valuations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pre-seed-investment-terms-calculator](https://vinkius.com/ai-agent-connect/pre-seed-investment-terms-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pre-Seed Investment Terms Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pre-seed-investment-terms-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pre-Seed Investment Terms Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pre-seed-investment-terms-calculator": {
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
