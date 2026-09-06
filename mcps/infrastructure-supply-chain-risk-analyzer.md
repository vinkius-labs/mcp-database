# Infrastructure Supply Chain Risk Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infrastructure-supply-chain-risk-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Quantify supply chain vulnerabilities, single-source exposure, and mitigation costs.

## Description
This MCP server provides specialized tools to assess infrastructure supply chain resilience. It allows AI agents to calculate supplier concentration risk, identify single-source exposure for critical components, estimate the financial impact of mitigation strategies, and determine supply recovery timelines. By using `calculate_concentration_risk`, `analyze_single_source_exposure`, `estimate_mitigation_costs`, and `evaluate_supply_recovery_timeline`, agents can pinpoint specific vulnerabilities in procurement and inventory management.


## Available Tools (4)
- **analyze_single_source_exposure**: Identifies the impact of relying on a single provider for specific items
- **calculate_concentration_risk**: Evaluates the risk score stemming from the distribution of supply among existing vendors
- **estimate_mitigation_costs**: Calculates the financial requirement to address identified supply chain gaps
- **evaluate_supply_recovery_timeline**: Determines the time window of vulnerability when a primary supplier is lost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infrastructure Supply Chain Risk Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the concentration risk if my suppliers have volumes of 60, 30, and 10 with a total volume of 100?"

**🤖 AI Agent:**
> The concentration risk score is high because 60% of the volume is held by a single supplier, indicating significant vulnerability.

---

**👤 You:**
> "Identify single-source exposure for a critical component named 'Microchip-A' with importance weight 0.9 that is currently single-sourced."

**🤖 AI Agent:**
> The single-source exposure for Microchip-A is high due to its critical importance weight of 0.9.

---

**👤 You:**
> "Calculate the supply gap if the primary lead time is 30 days, alternative lead time is 45 days, and I have 10 days of safety stock."

**🤖 AI Agent:**
> The supply gap is 35 days, as the 10 days of safety stock is insufficient to cover the 45-day alternative lead time.


## ❓ FAQ

**Q: How does the tool calculate concentration risk?**
The `calculate_concentration_risk` tool evaluates how procurement volume is distributed among vendors to identify systemic vulnerabilities.

**Q: Can I estimate the cost of adding new suppliers?**
Yes, you can use `estimate_mitigation_costs` to predict the financial investment required to onboard alternative suppliers and reduce risk.

**Q: How is the supply gap calculated?**
The `evaluate_supply_recovery_timeline` tool calculates the supply gap by comparing the time needed for backup suppliers to deliver against the available safety stock.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infrastructure-supply-chain-risk-analyzer](https://vinkius.com/ai-agent-connect/infrastructure-supply-chain-risk-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infrastructure Supply Chain Risk Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infrastructure-supply-chain-risk-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infrastructure Supply Chain Risk Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infrastructure-supply-chain-risk-analyzer": {
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
