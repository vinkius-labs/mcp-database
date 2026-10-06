# Household Waste Stream Audit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-waste-stream-audit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Calculate waste composition, category distribution, and diversion rates.

## Description
This MCP server provides tools to analyze household waste management efficiency. Use `analyze_waste_composition` to get a full breakdown of waste streams including landfill, recycling, compost, reuse, and hazardous categories. You can also use `get_stream_totals` to find the total weight, `compare_diversion_targets` to check if diversion goals are met, and `identify_primary_stream` to find the largest waste category.


## Available Tools (4)
- **compare_diversion_targets**: Evaluates if the current diversion rate meets or exceeds a specific target threshold
- **get_stream_totals**: Aggregates the raw weights of all streams into a single total weight value
- **identify_primary_stream**: Determines which waste stream represents the largest portion of the total waste
- **analyze_waste_composition**: Calculates the percentage distribution of each waste stream and the overall diversion rate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Waste Stream Audit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the composition of my waste if I have 50kg landfill, 30kg recycling, 10kg compost, 5kg reuse, and 5kg hazardous?"

**🤖 AI Agent:**
> The waste composition is: Landfill 50%, Recycling 30%, Compost 10%, Reuse 5%, and Hazardous 5%. Your diversion rate is 45%.

---

**👤 You:**
> "Which waste stream is my largest?"

**🤖 AI Agent:**
> The largest waste stream is Landfill with a weight of 100kg.

---

**👤 You:**
> "Did I meet my 50% diversion target with 40kg recycling, 20kg compost, 10kg reuse, and 30kg landfill?"

**🤖 AI Agent:**
> Yes, your current diversion rate is 50%, which meets your target.


## ❓ FAQ

**Q: How do I calculate the diversion rate?**
The diversion rate is calculated by summing the weights of recycling, compost, and reuse streams, then dividing by the total weight of all streams.

**Q: Can I check if I met my recycling goals?**
Yes, use the `compare_diversion_targets` tool to evaluate if your current diversion rate meets a specific target threshold.

**Q: What waste streams are supported?**
The server supports Landfill, Recycling, Compost, Reuse, and Hazardous waste streams.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-waste-stream-audit](https://vinkius.com/en/ai-agent-connect/household-waste-stream-audit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Waste Stream Audit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-waste-stream-audit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Waste Stream Audit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-waste-stream-audit": {
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
