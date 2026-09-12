# Crude Oil Assay Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/crude-oil-assay-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Analyze crude oil properties, yield distributions, and blend compatibility.

## Description
This MCP server provides essential tools for refinery planning and crude oil characterization. It allows AI agents to perform complex petroleum calculations, including `get_crude_classification` to categorize feedstock, `calculate_yield_distribution` to estimate product volumes from TBP data, `estimate_product_qualities` to predict refined properties, and `evaluate_blend_compatibility` to verify if mixing different crudes meets target specifications.


## Available Tools (4)
- **calculate_yield_distribution**: 
- **estimate_product_qualities**: 
- **evaluate_blend_compatibility**: 
- **get_crude_classification**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crude Oil Assay Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify a crude with 32 API gravity and 0.5% sulfur content."

**🤖 AI Agent:**
> The crude is classified as Light/Sweet.

---

**👤 You:**
> "What is the yield distribution for this TBP data: [{'temp': 100, 'vol': 10}, {'temp': 200, 'vol': 40}] with cuts [{'name': 'Naphtha', 'startTemp': 50, 'endTemp': 150}]?"

**🤖 AI Agent:**
> The Naphtha yield is 10%.

---

**👤 You:**
> "Predict qualities for crude with 30 API, 2.0% sulfur, and 15 cSt viscosity."

**🤖 AI Agent:**
> The estimated sulfur in distillates is 1.2% and the estimated viscosity index is 85.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can classify crude oil types, estimate product yields from distillation curves, predict product qualities, and check if crude blends meet specific targets.

**Q: How do I provide TBP data?**
TBP data should be provided as a JSON string containing objects with temperature and cumulative volume percentage.

**Q: Can I check if a blend is compatible?**
Yes, use the blend evaluation tool to determine if mixing two crudes will satisfy your target API, sulfur, or viscosity limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/crude-oil-assay-analysis](https://vinkius.com/en/ai-agent-connect/crude-oil-assay-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crude Oil Assay Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crude-oil-assay-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crude Oil Assay Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crude-oil-assay-analysis": {
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
