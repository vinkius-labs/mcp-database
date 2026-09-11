# Backfill Design Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/backfill-design-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design underground mine backfill mixes by calculating cement requirements and curing times.

## Description
This MCP server provides specialized engineering tools for designing underground mine backfill. It allows engineers to determine the fundamental composition of a mix using `calculate_mix_design`, predict hydration timelines with `estimate_curing_duration`, and verify material compatibility via `validate_tailings_suitability`. It also supports economic analysis through `compare_mix_economies` to find the most cost-effective binder solutions for hydraulic, paste, or rock fill applications.


## Available Tools (4)
- **calculate_mix_design**: Determines the fundamental composition of a backfill mix
- **compare_mix_economies**: Evaluates the cost-effectiveness of different mix designs for the same strength requirement
- **estimate_curing_duration**: Predicts how long it takes for a specific mix to reach its design strength
- **validate_tailings_suitability**: Checks if a specific set of tailings properties can effectively support the desired backfill type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Backfill Design Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a mix design for paste fill with a tailings density of 2.6, a void ratio of 0.4, and a target strength of 2.0 MPa."

**🤖 AI Agent:**
> The required cement content is 12.5% with a water-to-cement ratio of 0.65.

---

**👤 You:**
> "How many days will it take for a paste fill with 15% cement and a 0.6 water-to-cement ratio to reach 3.0 MPa?"

**🤖 AI Agent:**
> The estimated curing duration is 28 days to reach the target strength.

---

**👤 You:**
> "Is a particle size distribution of [0.01, 0.05, 0.1, 0.5] suitable for hydraulic fill?"

**🤖 AI Agent:**
> The tailings are suitable for hydraulic fill with a low risk level.


## ❓ FAQ

**Q: What types of backfill can I design?**
You can design hydraulic fill, paste fill, and rock fill using the `calculate_mix_design` tool.

**Q: How do I know if my tailings are suitable?**
Use the `validate_tailings_suitability` tool by providing the particle size distribution to check for risks and suitability.

**Q: Can I compare the costs of two different mixes?**
Yes, the `compare_mix_economies` tool evaluates the cost-effectiveness of different mix designs based on cement unit costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/backfill-design-calculator](https://vinkius.com/en/ai-agent-connect/backfill-design-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Backfill Design Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `backfill-design-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Backfill Design Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "backfill-design-calculator": {
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
