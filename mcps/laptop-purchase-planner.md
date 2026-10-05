# Laptop Purchase Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/laptop-purchase-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A decision-support system that ranks laptops based on workload, budget, and personal priorities.

## Description
This MCP server provides specialized tools to help users find the perfect laptop. By using `get_laptop_catalog`, you can browse available hardware. The `rank_laptops_for_user` tool analyzes technical specifications against your specific workload intensity and budget constraints. You can also use `calculate_portability_rating` to evaluate mobility or `compare_laptop_specs` to see a detailed side-by-side technical breakdown of two different models.


## Available Tools (4)
- **compare_laptop_specs**: Provides a side-by-side technical comparison between two specific laptops
- **get_laptop_catalog**: Provides a list of all available laptops in the database for inspection
- **rank_laptops_for_user**: Generates a ranked list of laptops tailored to specific user needs
- **calculate_portability_rating**: Computes a numerical score representing how mobile a specific laptop is


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Laptop Purchase Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find me the best laptops for heavy video editing with a budget of $2000."

**🤖 AI Agent:**
> The best options for your heavy workload under $2000 are the ProStream X1 and the WorkStation Z5, both featuring high-performance CPUs and dedicated GPUs.

---

**👤 You:**
> "Which is more portable: the LiteBook Air or the TravelMate?"

**🤖 AI Agent:**
> The LiteBook Air has a higher portability score due to its lower weight and larger battery capacity.

---

**👤 You:**
> "List all budget tier laptops available."

**🤖 AI Agent:**
> The available budget tier laptops are the EcoBook 14, the BasicTab Pro, and the StudentLite 13.


## ❓ FAQ

**Q: How does the ranking system work?**
The system uses `rank_laptops_for_user` to weigh performance, price, and portability based on your specific priority weights and workload requirements.

**Q: Can I filter laptops by price?**
Yes, you can set a maximum budget, and the system will automatically disqualify any laptop that exceeds that limit.

**Q: What information is included in a technical comparison?**
Using `compare_laptop_specs`, you can view a detailed comparison of CPU, RAM, storage, GPU, weight, battery capacity, price, and warranty.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/laptop-purchase-planner](https://vinkius.com/en/ai-agent-connect/laptop-purchase-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Laptop Purchase Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `laptop-purchase-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Laptop Purchase Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "laptop-purchase-planner": {
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
