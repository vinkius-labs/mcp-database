# North Star Metric Derivation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/north-star-metric-derivation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [product-management](../categories/product-management.md)

Decompose high-level value into a structured North Star Metric hierarchy.

## Description
This MCP server provides a strategic framework to bridge the gap between raw data and strategic direction. It allows AI agents to decompose high-level value delivery into a structured hierarchy of North Star Metrics (NSM), including mathematical formulas, metric trees, and leading indicators. Use `derive_nsm_structure` to generate the complete decomposition, `analyze_segment_alignment` to validate segment value, `identify_leading_indicators` to find predictive metrics, and `validate_growth_engine_fit` to ensure strategic compatibility with your growth model.


## Available Tools (4)
- **analyze_segment_alignment**: Evaluates how well the proposed NSM captures value across different customer segments
- **derive_nsm_structure**: Generates the complete strategic decomposition of the North Star Metric
- **identify_leading_indicators**: Isolates specific, actionable metrics that act as early warning signs for the NSM
- **validate_growth_engine_fit**: Ensures the derived NSM is compatible with the selected growth model and business type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **North Star Metric Derivation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a North Star Metric structure for a subscription SaaS where the value is monthly active users."

**🤖 AI Agent:**
> The North Star Metric formula is Monthly Active Users (MAU). The hierarchy includes Daily Active Users (DAU) as a leading indicator and feature engagement rates as input metrics.

---

**👤 You:**
> "Check if my NSM formula is compatible with a viral growth model."

**🤖 AI Agent:**
> The formula is compatible with the viral growth model as it captures the user loop and sharing frequency required for expansion.

---

**👤 You:**
> "Find leading indicators for a marketplace NSM based on transaction volume."

**🤖 AI Agent:**
> The primary leading indicators are successful match rates between buyers and sellers and the average time to complete a transaction.


## ❓ FAQ

**Q: How does the NSM derivation work?**
The tool uses a decomposition framework to transform input metrics into a logical NSM formula and a multi-tiered hierarchy of leading indicators.

**Q: Can I validate my growth model compatibility?**
Yes, you can use `validate_growth_engine_fit` to ensure your derived NSM aligns with your specific growth engine and business model.

**Q: What are leading indicators?**
Leading indicators are predictive, actionable metrics that signal future movement in your North Star Metric before the primary metric changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/north-star-metric-derivation](https://vinkius.com/en/ai-agent-connect/north-star-metric-derivation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **North Star Metric Derivation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `north-star-metric-derivation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **North Star Metric Derivation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "north-star-metric-derivation": {
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
