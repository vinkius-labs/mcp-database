# Atmospheric Distillation Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/atmospheric-distillation-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design atmospheric distillation units by calculating stages, yields, and energy requirements.

## Description
This MCP server provides engineering tools to design Atmospheric Distillation Units (ADU/CDU). It allows users to determine the necessary theoretical stages using `calculate_column_stages`, predict product yields with `estimate_product_yields`, optimize heat recovery via `optimize_pumparounds`, and calculate total heat requirements with `evaluate_energy_consumption`. It is designed to bridge crude oil assay data with precise column configurations.


## Available Tools (4)
- **optimize_pumparounds**: Calculates the optimal location and flow of heat removal to maximize energy efficiency
- **calculate_column_stages**: Determines the necessary number of theoretical stages to achieve separation
- **estimate_product_yields**: Predicts the volume of each product fraction produced from a specific crude
- **evaluate_energy_consumption**: Calculates the total heat required for the furnace and the cooling required for products and pumparounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Atmospheric Distillation Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the number of stages needed for a throughput of 50000 kg/h with specific assay data."

**🤖 AI Agent:**
> The required number of theoretical stages is 32, with a minimum of 24 stages.

---

**👤 You:**
> "What are the expected yields for this crude oil?"

**🤖 AI Agent:**
> The predicted yields are: Naphtha 15%, Kerosene 12%, Diesel 25%, Gas Oil 30%, and Residue 18%.

---

**👤 You:**
> "Calculate the energy consumption for the column design."

**🤖 AI Agent:**
> The total energy requirement is 450 MW, consisting of 380 MW furnace duty and 70 MW condenser duty.


## ❓ FAQ

**Q: What inputs are needed for column stage calculation?**
You need to provide the crude throughput, the assay data as a JSON string, and the target product specifications.

**Q: Can I optimize energy efficiency?**
Yes, you can use `optimize_pumparounds` to find the best locations for heat removal to maximize energy recovery.

**Q: How are product yields determined?**
Yields are calculated by integrating the boiling point distribution from your assay data over the specified cut points.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/atmospheric-distillation-design](https://vinkius.com/en/ai-agent-connect/atmospheric-distillation-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Atmospheric Distillation Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `atmospheric-distillation-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Atmospheric Distillation Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "atmospheric-distillation-design": {
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
