# Catalytic Reformer Design Suite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/catalytic-reformer-design-suite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemical-engineering](../categories/chemical-engineering.md)

Optimize catalytic reforming units for gasoline production and hydrogen yield.

## Description
This MCP server provides a complete suite of tools for designing and optimizing catalytic reforming units. It allows engineers to determine reactor configurations using `design_reformer_configuration`, predict chemical outputs with `calculate_yield_and_products`, estimate catalyst life via `estimate_regeneration_cycle`, and fine-tune parameters using `optimize_operating_conditions`. It bridges the gap between naphtha feed properties and high-octane gasoline production.


## Available Tools (4)
- **calculate_yield_and_products**: Predicts the chemical output of the reforming process
- **design_reformer_configuration**: Determines the physical and operational setup of the reforming unit
- **estimate_regeneration_cycle**: Predicts how long the catalyst can remain active before needing regeneration
- **optimize_operating_conditions**: Suggests adjustments to temperature or pressure to hit a target RON or maximize a specific byproduct


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Catalytic Reformer Design Suite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a configuration for a naphtha feed with 40% naphthenes and 30% paraffins, targeting a RON of 95 using a platinum-based catalyst in semi-regenerative mode."

**🤖 AI Agent:**
> The designed configuration includes 3 reactors with a total volume of 45m3, operating at a target temperature of 510°C and a pressure of 15 bar.

---

**👤 You:**
> "What will be the hydrogen yield for a configuration with 2 reactors and 20m3 volume per reactor?"

**🤖 AI Agent:**
> The predicted hydrogen yield for this configuration is 3.2 wt%.

---

**👤 You:**
> "How long will the catalyst last in a semi-regenerative unit with this configuration?"

**🤖 AI Agent:**
> The estimated regeneration cycle length is 450 days.


## ❓ FAQ

**Q: How do I start a new design?**
Start by using the `design_reformer_configuration` tool with your naphtha properties and target RON to establish the initial reactor setup.

**Q: Can I optimize for hydrogen production?**
Yes, you can use `optimize_operating_conditions` and set the priority to 'maximize_hydrogen' to adjust temperature and pressure.

**Q: Does this support continuous regeneration modes?**
Yes, the tools support both semi-regenerative and continuous regeneration modes in their configuration and estimation logic.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/catalytic-reformer-design-suite](https://vinkius.com/en/ai-agent-connect/catalytic-reformer-design-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Catalytic Reformer Design Suite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `catalytic-reformer-design-suite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Catalytic Reformer Design Suite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "catalytic-reformer-design-suite": {
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
