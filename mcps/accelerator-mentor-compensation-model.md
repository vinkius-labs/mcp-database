# Accelerator Mentor Compensation Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-mentor-compensation-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate mentor costs, equity dilution, and industry benchmarks.

## Description
This MCP server provides financial modeling tools for accelerator programs to manage mentor engagement economics. It allows AI agents to calculate the total monetary cost of a mentor using `get_total_mentor_cost`, determine the resulting equity dilution via `calculate_equity_dilution`, and verify if compensation packages align with industry standards using `get_compensation_benchmark`.


## Available Tools (3)
- **calculate_equity_dilution**: Calculates the percentage of company ownership allocated to the mentor
- **get_compensation_benchmark**: Determines if the proposed compensation package aligns with industry standards
- **get_total_mentor_cost**: Calculates the total monetary cost of engaging a mentor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Mentor Compensation Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for a Senior mentor working 20 hours at a $200 market rate?"

**🤖 AI Agent:**
> $4,000

---

**👤 You:**
> "If I offer $50,000 in a company valued at $1,000,000, what is the equity dilution?"

**🤖 AI Agent:**
> 5%

---

**👤 You:**
> "Is a $10,000 offer for a Mid-level mentor with Medium engagement fair?"

**🤖 AI Agent:**
> At Market


## ❓ FAQ

**Q: How do I calculate the total cost of a mentor?**
You can use the `get_total_mentor_cost` tool by providing the mentor's hours, the compensation type (cash or equity), the market rate, and their expertise level.

**Q: Can I check if my compensation offer is fair?**
Yes, the `get_compensation_benchmark` tool compares your proposed amount against industry standards based on expertise and engagement levels.

**Q: How is equity dilution calculated?**
The `calculate_equity_dilution` tool calculates dilution by dividing the cash-equivalent compensation value by the total company valuation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-mentor-compensation-model](https://vinkius.com/ai-agent-connect/accelerator-mentor-compensation-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Mentor Compensation Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-mentor-compensation-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Mentor Compensation Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-mentor-compensation-model": {
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
