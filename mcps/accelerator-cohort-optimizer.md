# Accelerator Cohort Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-cohort-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business](../categories/business.md)

Optimizes accelerator cohort sizes by balancing resource constraints and peer learning value.

## Description
This MCP server provides specialized tools to determine the ideal number of participants for accelerator programs. It balances physical and financial constraints--such as desk space and funding--against the qualitative benefits of the network effect. Use `find_optimal_size` to identify the best cohort size for graduation success, `verify_resource_constraints` to check if a proposed size is feasible, and `calculate_network_effect_value` to estimate the peer learning benefits of a specific cohort size.


## Available Tools (3)
- **calculate_network_effect_value**: Estimates the qualitative "Peer Learning Value" gained from increasing the cohort size
- **find_optimal_size**: Determines the single best cohort size that maximizes the balance between resource efficiency and graduation success
- **verify_resource_constraints**: Validates if a specific proposed cohort size is feasible given the current operational limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Cohort Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best cohort size for a program with 50 desk spaces, 10 mentors, and $100,000 in funding?"

**🤖 AI Agent:**
> The optimal cohort size is 42 participants, which utilizes 84% of your desk space and maintains a high graduation success rate.

---

**👤 You:**
> "Is a cohort of 60 participants feasible if I only have 50 desks available?"

**🤖 AI Agent:**
> No, a cohort of 60 is not feasible because it exceeds the available desk space.

---

**👤 You:**
> "What is the peer learning value for a cohort of 20 people with a base value of 100?"

**🤖 AI Agent:**
> The total value for a cohort of 20 participants is 2,400.


## ❓ FAQ

**Q: How does the tool handle physical constraints?**
The `verify_resource_constraints` tool checks the proposed size against your available desk space and total program capacity to ensure feasibility.

**Q: Can I calculate the value of peer networking?**
Yes, you can use `calculate_network_effect_value` to estimate the total value gained from peer-to-peer interaction as the cohort size increases.

**Q: What determines the optimal cohort size?**
The `find_optimal_size` tool calculates the ideal size by finding the point where graduation success is maximized within your budget, mentor ratio, and capacity limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-cohort-optimizer](https://vinkius.com/ai-agent-connect/accelerator-cohort-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Cohort Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-cohort-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Cohort Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-cohort-optimizer": {
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
