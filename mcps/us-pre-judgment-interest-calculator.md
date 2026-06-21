# US Pre-judgment Interest Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-pre-judgment-interest-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate statutory pre-judgment interest for US states based on debt amount, default date, and state law.

## Description
This MCP server provides a precise engine to calculate statutory pre-judgment interest across various US jurisdictions. By using tools like `get_state_statute_details`, `calculate_accumulated_interest`, and `list_supported_juris_dictions`, AI agents can determine the legal interest rates (Simple or Compound) for specific states such as California, New York, or Texas. It handles complex date arithmetic to find the exact days elapsed between a default date and a reference date, ensuring compliance with state-specific statutes.


## Available Tools (3)
- **calculate_accumulated_interest**: Calculate total interest accrued on a debt
- **get_state_statute_details**: Get the legal interest rules for a specific state
- **list_supported_jurisdictions**: List all supported US states


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Pre-judgment Interest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the legal interest rate for California?"

**🤖 AI Agent:**
> The annual statutory interest rate for California is 7%, and it uses the Simple interest calculation method.

---

**👤 You:**
> "Calculate interest for a $10,000 debt in New York that defaulted on 2023-01-01, as of 2024-01-01."

**🤖 AI Agent:**
> $900.00 in total interest has accrued over 365 days.

---

**👤 You:**
> "Which states can I check for interest rates?"

**🤖 AI Agent:**
> The supported jurisdictions include California, New York, and Texas.


## ❓ FAQ

**Q: How do I know which states are supported?**
You can use the `list_supported_jurisdictions` tool to retrieve a complete list of all US states currently implemented in the calculator.

**Q: Does the calculation support compound interest?**
Yes, the engine applies either Simple or Compound interest based on the specific statute of the state provided. For example, Texas uses Compound interest.

**Q: What inputs are required for calculating interest?**
To use `calculate_accumulated_interest`, you must provide the debt amount, the default date (ISO 8601), a reference date (ISO 8601), and the name of the US state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-pre-judgment-interest-calculator](https://vinkius.com/mcp/us-pre-judgment-interest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Pre-judgment Interest Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-pre-judgment-interest-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Pre-judgment Interest Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-pre-judgment-interest-calculator": {
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
