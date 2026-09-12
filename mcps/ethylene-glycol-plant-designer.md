# Ethylene Glycol Plant Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/ethylene-glycol-plant-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Chemical engineering tool for modeling ethylene glycol production and reactor design.

## Description
This MCP server provides specialized chemical engineering tools to design and optimize ethylene glycol production plants. It allows users to calculate reactor specifications using `calculate_reactor_design`, estimate product yields with `predict_product_distribution`, determine distillation conditions via `optimize_separation_parameters`, and assess financial feasibility with `evaluate_plant_economics`. The tools model the hydration of ethylene oxide and the subsequent separation of MEG, DEG, and TEG.


## Available Tools (4)
- **evaluate_plant_economics**: Assesses the feasibility of a design based on throughput and product mix
- **calculate_reactor_design**: Determines the required reactor physical specifications based on feedstock and target output
- **optimize_separation_parameters**: Provides the necessary operating conditions for the distillation train to achieve a specific product purity
- **predict_product_distribution**: Estimates the yield of MEG, DEG, and TEG


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ethylene Glycol Plant Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reactor design for 500 units of EO with a water-to-EO ratio of 10 and a target capacity of 1000."

**🤖 AI Agent:**
> The required reactor volume is 1250 m³, with a residence time of 45 minutes and a heat duty of 450 MW.

---

**👤 You:**
> "What is the expected product distribution if the water-to-EO ratio is 15 and residence time is 60 minutes?"

**🤖 AI Agent:**
> The expected yield is 85% MEG, 12% DEG, and 3% TEG.

---

**👤 You:**
> "Estimate the plant economics for a design with 1000 units of capacity and EO cost of 50 per unit."

**🤖 AI Agent:**
> The projected gross margin is $250,000 with an operating cost of $150,000 and revenue of $400,000.


## ❓ FAQ

**Q: How do I calculate the reactor volume?**
You can use the `calculate_reactor_design` tool by providing the available ethylene oxide, the target plant capacity, and the desired water-to-EO ratio.

**Q: Can I predict the yield of MEG, DEG, and TEG?**
Yes, the `predict_product_distribution` tool estimates the yield of Monoethylene Glycol, Diethylene Glycol, and Triethylene Glycol based on the water-to-EO ratio and residence time.

**Q: How is the economic feasibility assessed?**
The `evaluate_plant_economics` tool calculates operating costs, revenue, and gross margin using the reactor design, product distribution, and feedstock costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/ethylene-glycol-plant-designer](https://vinkius.com/en/ai-agent-connect/ethylene-glycol-plant-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ethylene Glycol Plant Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ethylene-glycol-plant-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ethylene Glycol Plant Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ethylene-glycol-plant-designer": {
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
