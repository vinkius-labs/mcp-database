# Decline Curve Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/decline-curve-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Forecast oil and gas production using Arps decline equations.

## Description
This MCP server provides specialized tools for petroleum engineers to perform Decline Curve Analysis (DCA). By applying Arps equations, users can determine the best-fit decline parameters from historical data using `fit_decline_curve`. The server allows for predicting future production rates with `forecast_production`, calculating total recoverable volumes via `calculate_reserves`, and verifying if a well has reached the necessary Boundary-Dominated Flow regime using `validate_flow_regime`.


## Available Tools (4)
- **validate_flow_regime**: Analyzes historical data to determine if the well has transitioned to boundary-dominated flow
- **calculate_reserves**: Calculates the total recoverable volume and the remaining volume available
- **fit_decline_curve**: Determines the best-fit decline parameters from historical production data
- **forecast_production**: Predicts future production rates for a specific future time point


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Decline Curve Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you find the best-fit decline parameters for this production data: [{"timestamp": 1672531200, "rate": 1000}, {"timestamp": 1675209600, "rate": 850}, {"timestamp": 1677628800, "rate": 720}] using a hyperbolic model?"

**🤖 AI Agent:**
> The best-fit parameters for the hyperbolic model are a decline rate of 0.15 and a b-factor of 0.5, with a fit quality score of 0.98.

---

**👤 You:**
> "Based on a decline rate of 0.1 and a b-factor of 0.4, what will the production rate be at time 12 months?"

**🤖 AI Agent:**
> The forecasted production rate at 12 months is 450 barrels per day.

---

**👤 You:**
> "What is the remaining reserve if the EUR is 1,000,000 and we have already produced 300,000?"

**🤖 AI Agent:**
> The remaining reserves are 700,000 units.


## ❓ FAQ

**Q: What types of decline models are supported?**
The server supports exponential, hyperbolic, and harmonic decline models through the `fit_decline_curve` tool.

**Q: How do I know if my data is valid for forecasting?**
You should use `validate_flow_regime` to ensure the production data has transitioned from transient flow to boundary-dominated flow before applying Arps equations.

**Q: Can I calculate the total recoverable volume?**
Yes, the `calculate_reserves` tool calculates both the Estimated Ultimate Recovery (EUR) and the remaining reserves.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/decline-curve-analysis](https://vinkius.com/en/ai-agent-connect/decline-curve-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Decline Curve Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `decline-curve-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Decline Curve Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "decline-curve-analysis": {
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
