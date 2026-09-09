# Drilling Cost Per Foot Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/drilling-cost-per-foot-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate drilling cost per foot and perform sensitivity analysis for ROP and bit life.

## Description
This MCP server provides essential economic analysis tools for drilling operations. Use `calculate_cpf` to determine the primary cost per foot and total well cost based on rig rates, bit costs, and drilling/trip times. Perform sensitivity testing with `analyze_rop_sensitivity` to see how changes in the rate of penetration impact efficiency, or use `analyze_bit_life_sensitivity` to evaluate the impact of bit durability. You can also use `estimate_formation_impact` to adjust performance parameters based on rock hardness (soft, medium, or hard).


## Available Tools (4)
- **analyze_bit_life_sensitivity**: Evaluates how the durability of the bit impacts the overall cost efficiency
- **analyze_rop_sensitivity**: Evaluates how changes in drilling speed impact the overall cost efficiency
- **calculate_cpf**: Determines the primary economic metric of the drilling operation
- **estimate_formation_impact**: Provides a quick estimation of how different rock types affect drilling parameters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drilling Cost Per Foot Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost per foot for a 5000ft interval with a $500/hr rig rate, $5000 bit cost, 100 hours of drilling, and 20 hours of trip time."

**🤖 AI Agent:**
> The cost per foot for this interval is $12.00, with a total well cost of $60,000.

---

**👤 You:**
> "What happens to the cost per foot if my ROP increases by 15%? My current CPF is $12.00, ROP is 50 ft/hr, rig rate is $500/hr, bit cost is $5000, trip time is 20 hours, bit life is 500 ft, and total footage is 5000 ft."

**🤖 AI Agent:**
> An increase of 15% in ROP results in a new cost per foot of $10.85, which is a 9.58% reduction in cost.

---

**👤 You:**
> "Estimate the impact of moving from a medium to a hard formation if my base ROP is 50 ft/hr and bit life is 500 ft."

**🤖 AI Agent:**
> In a hard formation, the adjusted ROP is 25.0 ft/hr and the adjusted bit life is 250.0 ft.


## ❓ FAQ

**Q: How do I calculate the basic cost per foot?**
Use the `calculate_cpf` tool by providing the rig rate, bit cost, drilling time, trip time, and total footage.

**Q: Can I test how a faster drilling speed affects my budget?**
Yes, use the `analyze_rop_sensitivity` tool to input your current ROP and a percentage change to see the impact on cost per foot.

**Q: How does formation type affect my results?**
You can use `estimate_formation_impact` to adjust your baseline ROP and bit life based on whether the formation is soft, medium, or hard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/drilling-cost-per-foot-analyzer](https://vinkius.com/ai-agent-connect/drilling-cost-per-foot-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drilling Cost Per Foot Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drilling-cost-per-foot-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drilling Cost Per Foot Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drilling-cost-per-foot-analyzer": {
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
