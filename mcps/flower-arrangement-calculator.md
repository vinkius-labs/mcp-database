# Flower Arrangement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/flower-arrangement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Deterministic floral design engine for precise stem counts and mechanical supplies.

## Description
This MCP server provides professional floral designers with a deterministic engine to calculate exact botanical and mechanical requirements. By inputting arrangement types, container sizes, and design styles, users receive precise stem counts for focal flowers, secondary blooms, fillers, and greens, alongside necessary mechanical supplies like floral foam or chicken wire. Use `calculate_single_arrangement` for individual pieces or `calculate_wedding_order` to generate master procurement lists for entire wedding parties.


## Available Tools (3)
- **get_design_density_multiplier**: Retrieves the density factor used to translate physical size into stem count
- **calculate_single_arrangement**: Calculates the exact botanical and mechanical requirements for one specific floral piece
- **calculate_wedding_order**: Calculates total requirements for an entire wedding party based on headcount and specific roles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flower Arrangement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many stems do I need for a round bouquet with a 20cm container?"

**🤖 AI Agent:**
> For a 20cm round bouquet, you will need 5 focal stems, 7 secondary stems, 7 filler stems, and 5 greens stems.

---

**👤 You:**
> "Calculate a wedding order with a bridal bouquet, 3 bridesmaids, and 5 centerpieces."

**🤖 AI Agent:**
> Your wedding order requires 42 focal stems, 63 secondary stems, 63 filler stems, 42 greens stems, and 5 units of floral foam.

---

**👤 You:**
> "What is the density multiplier for a cascading style?"

**🤖 AI Agent:**
> The density multiplier for the cascading style is 1.5.


## ❓ FAQ

**Q: How are the stem counts calculated?**
The engine uses a deterministic ratio model: 20% focal flowers, 30% secondary flowers, 30% filler flowers, and 20% greens, scaled by the container size and design style density.

**Q: Can I plan an entire wedding floral order at once?**
Yes, you can use the `calculate_wedding_order` tool to generate a master procurement list covering bridal bouquets, bridesmaids, centerpieces, arches, and boutonnieres.

**Q: What design styles are supported?**
The supported styles are round, cascading, linear, and garden-style. You can use `get_design_density_multiplier` to see how each style affects the volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/flower-arrangement-calculator](https://vinkius.com/ai-agent-connect/flower-arrangement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flower Arrangement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flower-arrangement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flower Arrangement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flower-arrangement-calculator": {
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
