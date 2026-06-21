# Bullwhip Effect Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bullwhip-effect-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Quantify demand amplification and identify instability patterns in supply chains.

## Description
The Bullwhip Effect Calculator allows you to measure how demand fluctuations increase as they move upstream through the supply chain. Using tools like `get_segment_amplification`, you can calculate the amplification ratio between specific stages. You can also use `assess_chain_severity` to evaluate overall health (Low, Medium, or Severe) and `identify_instability_source` to pinpoint which tier--Retailer, Distributor, or Manufacturer--is driving variance increases.


## Available Tools (3)
- **assess_chain_severity**: Evaluates the overall health of the supply chain by classifying the total cumulative amplification
- **get_segment_amplification**: If downstream <= upstream, ratio is 1.

Determines the specific amplification ratio for a single transition between two supply chain stages
- **identify_instability_source**: Identifies which specific tier in the supply chain is most responsible for amplification


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bullwhip Effect Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the amplification ratio between a retailer with 10 units of demand variance and a distributor with 25 units of order variance."

**🤖 AI Agent:**
> The amplification ratio is 2.50x.

---

**👤 You:**
> "Assess the severity of a supply chain where the first segment ratio is 1.2 and the second is 3.5."

**🤖 AI Agent:**
> The supply chain severity is classified as Severe due to the high amplification in the second segment.

---

**👤 You:**
> "Identify the source of instability given consumer variance 5, retailer 10, distributor 40, and manufacturer 100."

**🤖 AI Agent:**
> The primary driver of instability is the Manufacturer tier.


## ❓ FAQ

**Q: What is the Bullwhip Effect?**
It is a phenomenon where small fluctuations in consumer demand cause progressively larger fluctuations in orders as they move upstream through the supply chain.

**Q: How do I calculate the amplification ratio?**
Use the `get_segment_amplification` tool by providing the upstream variance and downstream variance.

**Q: Can this tool identify the cause of instability?**
Yes, the `identify_instability_source` tool analyzes variance patterns to find which tier is the primary driver of demand distortion.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bullwhip-effect-calculator](https://vinkius.com/mcp/bullwhip-effect-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bullwhip Effect Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bullwhip-effect-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bullwhip Effect Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bullwhip-effect-calculator": {
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
