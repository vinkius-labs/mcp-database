# Donation vs Disposal Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/donation-vs-disposal-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Compare the economic and environmental impact of donation, resale, recycling, and disposal.

## Description
This MCP server provides decision-support tools to evaluate end-of-life pathways for goods. Use `compare_pathways` to see a side-by-side comparison of financial, environmental, and circularity impacts. You can also use `calculate_environmental_impact` to study carbon footprints, `calculate_economic_efficiency` to determine net monetary returns, and `get_diversion_summary` to measure waste avoidance.


## Available Tools (4)
- **calculate_environmental_impact**: Isolates the carbon footprint calculation to study how transport distance affects the environment
- **compare_pathways**: Provides a side-by-side comparison of all possible end-of-life options for a specific item
- **get_diversion_summary**: Answers how much waste is avoided across different scenarios
- **calculate_economic_efficiency**: Determines which pathway provides the highest monetary return or lowest cost


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Donation vs Disposal Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the impact of donating vs recycling a 10kg item with 5km transport and 0.5 emissions factor."

**🤖 AI Agent:**
> Donation results in a net financial impact of $0.00 with 10kg diverted. Recycling results in a net financial impact of -$5.00 with 8kg diverted.

---

**👤 You:**
> "What is the carbon footprint for a 50km trip with an emissions factor of 0.2?"

**🤖 AI Agent:**
> The total carbon footprint is 10.0 units.

---

**👤 You:**
> "Calculate the economic efficiency for a resale with $50 revenue and $10 total fees."

**🤖 AI Agent:**
> The net balance is $40.00.


## ❓ FAQ

**Q: How do I compare different disposal options?**
Use the `compare_pathways` tool with your item's weight, transport distance, and relevant fees to get a full comparison.

**Q: Can I calculate the carbon footprint of transport?**
Yes, the `calculate_environmental_impact` tool allows you to isolate and calculate total emissions based on distance and emissions factors.

**Q: How is waste avoidance measured?**
The `get_diversion_summary` tool calculates the total mass diverted from the waste stream based on the chosen pathways.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/donation-vs-disposal-comparator](https://vinkius.com/en/ai-agent-connect/donation-vs-disposal-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Donation vs Disposal Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `donation-vs-disposal-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Donation vs Disposal Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "donation-vs-disposal-comparator": {
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
