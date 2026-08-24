# Beekeeping Harvest Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/beekeeping-harvest-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deterministic honey yield, storage, and wax byproduct estimation.

## Description
This MCP server provides precise tools for beekeepers to estimate honey harvests. Use `calculate_honey_yield` to determine extractable honey weight and check moisture safety. Use `estimate_storage_needs` to plan jar requirements, `calculate_wax_byproduct` to predict wax yields, and `suggest_super_timing` to manage hive space based on nectar flow.


## Available Tools (4)
- **suggest_super_timing**: Recommends when to add new supers to the hive based on the nectar flow environment
- **calculate_honey_yield**: Determines the total weight of honey and the extractable amount based on equipment and capping status
- **calculate_wax_byproduct**: Estimates the amount of beeswax generated from the harvested cappings
- **estimate_storage_needs**: Calculates how many standard jars are required to store the expected harvest


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beekeeping Harvest Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 10 deep frames that are 80% capped. The moisture is 17%. How much honey can I harvest?"

**🤖 AI Agent:**
> You can harvest 24kg of honey from your 10 deep frames.

---

**👤 You:**
> "How many 1kg jars do I need for 15kg of honey?"

**🤖 AI Agent:**
> You will need 15 jars of 1kg capacity.

---

**👤 You:**
> "The nectar flow is heavy. What should I do?"

**🤖 AI Agent:**
> Add Super Now. You should add equipment immediately to prevent swarming or honey starvation.


## ❓ FAQ

**Q: How do I know if my honey is safe from fermentation?**
You can use the `calculate_honey_yield` tool. It includes a safety check that flags if the moisture content exceeds the threshold that risks fermentation.

**Q: Can I estimate how many jars I need to buy?**
Yes, after calculating your extractable honey weight, use the `estimate_storage_needs` tool to get the exact count for both 500g and 1kg jars.

**Q: How does frame type affect the calculation?**
The tools account for standard capacities: deep frames (~3kg), medium frames (~2kg), and shallow frames (~1kg). You specify the type in `calculate_honey_yield` or `calculate_wax_byproduct`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/beekeeping-harvest-calculator](https://vinkius.com/ai-agent-connect/beekeeping-harvest-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beekeeping Harvest Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beekeeping-harvest-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beekeeping Harvest Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beekeeping-harvest-calculator": {
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
