# Alkylation Unit Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/alkylation-unit-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design high-octane gasoline components by calculating reactor dimensions, yields, and acid economics.

## Description
This MCP server provides specialized engineering tools for designing alkylation units used in refinery operations. It allows AI agents to calculate critical parameters for producing high-octane alkylate from olefin feeds. Users can determine physical reactor requirements using `calculate_reactor_dimensions`, predict product quality with `estimate_yield_and_octane`, evaluate operational costs via `calculate_acid_economics`, and find optimal process settings through `optimize_unit_configuration`. The tools account for different catalyst types, including sulfuric and hydrofluoric acid, to ensure accurate modeling of yield and octane numbers.


## Available Tools (4)
- **calculate_reactor_dimensions**: Determines the physical size of the reactor required for a given production target
- **estimate_yield_and_octane**: Predicts the quality and quantity of the resulting alkylate
- **optimize_unit_configuration**: Suggests the best combination of feed and catalyst to meet a specific octane target
- **calculate_acid_economics**: Estimates the operational cost and volume of acid required for the process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alkylation Unit Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required reactor volume for an olefin feed rate of 50 with an isobutane ratio of 1.5 using sulfuric acid?"

**🤖 AI Agent:**
> The required reactor volume is 1250 cubic meters with a residence time of 4.5 hours.

---

**👤 You:**
> "Estimate the yield and octane number for a feed rate of 100, isobutane ratio of 2.0, and hydrofluoric acid."

**🤖 AI Agent:**
> The expected alkylate yield is 94% with an octane number of 96.5.

---

**👤 You:**
> "Help me optimize my unit to reach an octane of 95 using 500 units of available isobutane and sulfuric acid."

**🤖 AI Agent:**
> To reach an octane of 95, the recommended isobutane ratio is 1.8, which results in an expected yield of 92% and an estimated reactor volume of 850 cubic meters.


## ❓ FAQ

**Q: How do I calculate the required reactor size?**
You can use the `calculate_reactor_dimensions` tool by providing the olefin feed rate, the isobutane ratio, and the catalyst type.

**Q: Can I optimize for a specific octane target?**
Yes, the `optimize_unit_configuration` tool helps find the best isobutane ratio and reactor volume to meet your desired octane rating.

**Q: Does this tool support both sulfuric and hydrofluoric acid models?**
Yes, all tools like `calculate_acid_economics` and `estimate_yield_and_octane` allow you to specify either sulfuric or hydrofluoric acid as the catalyst type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/alkylation-unit-design](https://vinkius.com/en/ai-agent-connect/alkylation-unit-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alkylation Unit Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `alkylation-unit-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alkylation Unit Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alkylation-unit-design": {
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
