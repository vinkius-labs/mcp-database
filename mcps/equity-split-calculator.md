# Equity Split Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/equity-split-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate fair ownership distribution among co-founders using weighted factors or dynamic slicing.

## Description
The Equity Split Calculator removes ambiguity from equity negotiations by transforming subjective contributions into objective, measurable shares. Using the `calculate_weighted_split` tool, you can distribute equity based on fixed importance weights applied to pillars like Idea, Execution, Capital, Risk, and Dedication. Alternatively, use `calculate_dynamic_slices` to convert raw physical contributions (hours, dollars, etc.) into enterprise 'slices' using assigned multipliers. Finally, the `generate_equity_audit` tool provides a qualitative and quantitative justification for why a specific distribution was reached, highlighting the reasoning behind the numbers.


## Available Tools (3)
- **calculate_dynamic_slices**: Multipliers are applied to cash, IP, equipment, and time.

Converts raw contributions into slices using multipliers
- **generate_equity_audit**: Generates a qualitative justification for the calculated equity
- **calculate_weighted_split**: Weights must sum to 1.

Calculates equity distribution based on fixed pillar weights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Equity Split Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate an equity split where Founder A has scores of 10 for idea and 5 for execution, and Founder B has 5 for idea and 10 for execution. Use equal weights for both pillars."

**🤖 AI Agent:**
> Founder A: 50%, Founder B: 50%. Both founders contributed a total of 15 weighted points, resulting in an equal split.

---

**👤 You:**
> "Using `calculate_dynamic_slices`, what is the share for Alice if she contributed $1000 in Cash (multiplier 2) and Bob contributed 50 hours of Time (multiplier 1)?"

**🤖 AI Agent:**
> Alice has 2000 slices and Bob has 50 slices. Alice's share is approximately 97.56% and Bob's share is approximately 2.44%.

---

**👤 You:**
> "Generate an audit report for a distribution where Founder C has 70% ownership due to high capital investment."

**🤖 AI Agent:**
> Founder C's 70% ownership is justified by their significant capital contribution, which provided the necessary liquidity for early-stage operations and mitigated initial financial risk.


## ❓ FAQ

**Q: What is the difference between the weighted and dynamic methods?**
The weighted method uses fixed importance scores for pillars like execution or capital, while the dynamic method (Slicing Pie) converts ongoing contributions into slices using multipliers.

**Q: How do I use `calculate_dynamic_slices`?**
Provide a JSON array of contributions, where each entry includes the founder's name, the type (e.g., Cash, Time), and the amount contributed.

**Q: Can I justify my equity split?**
Yes, use the `generate_equity_audit` tool to create a report that explains the quantitative results through qualitative justifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/equity-split-calculator](https://vinkius.com/mcp/equity-split-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Equity Split Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `equity-split-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Equity Split Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "equity-split-calculator": {
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
