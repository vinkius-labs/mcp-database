# Hydrocracker Unit Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hydrocracker-unit-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for sizing hydrocracker reactors, estimating hydrogen demand, and predicting product yields.

## Description
This MCP server provides specialized engineering capabilities for hydrocracking unit design. It allows users to calculate critical reactor parameters using `calculate_reactor_sizing`, predict hydrogen requirements via `estimate_hydrogen_demand`, and model product distributions with `generate_product_yields`. Additionally, it can validate if the resulting products meet refinery standards through `evaluate_product_quality`.


## Available Tools (4)
- **calculate_reactor_sizing**: Determines the physical dimensions required for the reactor vessel
- **estimate_hydrogen_demand**: Predicts the total hydrogen consumption for the process
- **evaluate_product_quality**: Checks if the predicted products meet specific refinery quality standards
- **generate_product_yields**: Predicts the volume and mass of each product in the final slate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydrocracker Unit Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required reactor volume for a feed flow rate of 5000 kg/h at 0.8 conversion severity and 400 degrees Celsius?"

**🤖 AI Agent:**
> The required reactor volume is 125.5 m³ with a residence time of 2.5 hours and a catalyst mass of 85,000 kg.

---

**👤 You:**
> "Estimate the hydrogen demand for 10000 kg/h of feed with 0.5% sulfur and 0.1% nitrogen at 0.7 conversion severity."

**🤖 AI Agent:**
> The total hydrogen consumption is 450 kg/h with a hydrogen utilization ratio of 0.85.

---

**👤 You:**
> "What will the product yields be for a 2000 kg/h feed at 0.9 conversion severity with a target slate of 40% naphtha and 60% diesel?"

**🤖 AI Agent:**
> The predicted yields are 800 kg/h of naphtha and 1200 kg/h of diesel, totaling 2000 kg/h.


## ❓ FAQ

**Q: How do I determine the required reactor size?**
You can use the `calculate_reactor_sizing` tool by providing the feedstock mass flow rate, the intended conversion severity, and the operating temperature.

**Q: Can I predict the hydrogen needed for my specific feedstock?**
Yes, the `estimate_hydrogen_demand` tool calculates hydrogen consumption based on feed flow rate, sulfur and nitrogen content, and conversion severity.

**Q: How can I check if my diesel meets quality targets?**
Use the `evaluate_product_quality` tool to verify if the predicted products meet specific metrics like cetane number or distillation ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hydrocracker-unit-design](https://vinkius.com/en/ai-agent-connect/hydrocracker-unit-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydrocracker Unit Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydrocracker-unit-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydrocracker Unit Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydrocracker-unit-design": {
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
