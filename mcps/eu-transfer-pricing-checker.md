# EU Transfer Pricing Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-transfer-pricing-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Verify intercompany transaction compliance with OECD Arm's Length Principle using industry benchmarks.

## Description
The EU Transfer Pricing Checker is a specialized compliance engine designed to ensure that intercompany transactions between related entities adhere to the OECD Arm's Length Principle. By comparing applied margins against industry-standard benchmarks, it identifies potential tax adjustment risks. AI agents can use tools like `check_compliance` to verify if a specific margin falls within established ranges, `evaluate_risk_impact` to assess the severity of deviations, and `get_benchmark_ranges` to retrieve market-standard minimum and maximum thresholds for various sectors and functions.


## Available Tools (3)
- **check_compliance**: Checks if a transaction margin falls within the established arm's length range
- **evaluate_risk_impact**: Determines the level of tax audit risk and potential severity
- **get_benchmark_ranges**: Retrieves the hardcoded market-standard ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Transfer Pricing Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if a 5% margin in the Manufacturing sector for Distribution using TNMM is compliant."

**🤖 AI Agent:**
> The `check_compliance` tool will analyze the 5% margin against the Manufacturing/Distribution benchmark for TNMM and return whether it falls within the arm's length range.

---

**👤 You:**
> "What is the tax risk if my applied margin is 15% in Technology/Services using Cost Plus?"

**🤖 AI Agent:**
> By calling `evaluate_risk_impact`, you can determine the specific risk level (Low, Medium, or High) and the potential severity of a tax adjustment for that 15% margin.

---

**👤 You:**
> "Show me all available benchmark ranges for the Retail sector in Logistics."

**🤖 AI Agent:**
> The `get_benchmark_ranges` tool will return a list of all recognized transfer pricing methods and their corresponding min/max margins for the Retail sector in Logistics.


## ❓ FAQ

**Q: How can I check if my transaction margin is compliant?**
Use the `check_compliance` tool by providing the industrial sector, business function, transfer pricing method (CUP, Cost Plus, or TNMM), and the applied margin percentage.

**Q: What does the risk impact evaluation represent?**
The `evaluate_risk_impact` tool calculates the level of tax audit risk and potential severity of a fiscal adjustment based on how far your applied margin deviates from the benchmark median.

**Q: Where can I find the standard market ranges?**
You can retrieve predefined industry-standard minimum and maximum margins using the `get_benchmark_ranges` tool for specific sectors and functions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-transfer-pricing-checker](https://vinkius.com/mcp/eu-transfer-pricing-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EU Transfer Pricing Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eu-transfer-pricing-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EU Transfer Pricing Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eu-transfer-pricing-checker": {
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
