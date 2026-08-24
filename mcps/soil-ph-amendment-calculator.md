# Soil pH Amendment Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/soil-ph-amendment-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate precise soil amendment amounts and costs based on soil type and pH targets.

## Description
This MCP server provides deterministic tools for managing soil chemistry. Use `calculate_amendment_requirement` to determine the exact weight of lime or sulfur needed for your specific soil texture (sand, loam, or clay) and area. You can also use `estimate_amendment_cost` to project total expenses and `get_soil_compatibility` to verify if an amendment matches your pH adjustment goals. It automatically accounts for soil buffering capacity and enforces safe incremental pH changes.


## Available Tools (3)
- **calculate_amendment_requirement**: Determines the specific quantity of amendment needed to reach a target pH within safe limits
- **estimate_amendment_cost**: Calculates the financial cost of the required amendment based on market pricing
- **get_soil_compatibility**: Answers whether a specific amendment is chemically appropriate for the user's goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Soil pH Amendment Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 500 sq ft of clay soil with a pH of 5.5. I want to reach a pH of 6.5. How much lime do I need?"

**🤖 AI Agent:**
> To raise the pH from 5.5 to 6.5 in 500 sq ft of clay soil, you will need 120 lbs of calcitic lime. Since this is a 1.0 unit change, it can be applied in 1 step.

---

**👤 You:**
> "How much will it cost to buy 50 lbs of elemental sulfur at $2.50 per lb?"

**🤖 AI Agent:**
> The total cost for 50 lbs of elemental sulfur at $2.50 per lb is $125.00.

---

**👤 You:**
> "Is aluminum sulfate a good choice if I want to lower my soil pH?"

**🤖 AI Agent:**
> Yes, aluminum sulfate is a compatible amendment for lowering soil pH.


## ❓ FAQ

**Q: How does soil type affect the calculation?**
The tool accounts for buffering capacity. For example, clay soil requires more amendment than sand to achieve the same pH shift.

**Q: Can I change my soil pH by more than 1.0 unit at once?**
No. To protect soil microbiology, the tool calculates the `requiredSteps` to ensure you never exceed a 1.0 pH unit change per application.

**Q: What amendments can I use to raise pH?**
You can use calcitic lime or dolomitic lime. You can verify compatibility using the `get_soil_compatibility` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/soil-ph-amendment-calculator](https://vinkius.com/ai-agent-connect/soil-ph-amendment-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Soil pH Amendment Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `soil-ph-amendment-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Soil pH Amendment Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "soil-ph-amendment-calculator": {
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
