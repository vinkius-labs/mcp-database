# SAFE Conversion Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/safe-conversion-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate SAFE conversion metrics, dilution impact, and pro-rata rights.

## Description
This MCP server provides a specialized financial calculation engine for SAFE (Simple Agreement for Future Equity) instruments. It allows AI agents to determine precise equity outcomes following priced rounds. Use `calculate_basic_conversion` to find conversion prices and ownership, `simulate_dilution_impact` to model how new capital affects existing holders, and `apply_pro_rata_rights` to calculate necessary investments to maintain ownership stakes. It also supports `compare_safe_versions` to analyze different term scenarios.


## Available Tools (4)
- **apply_pro_rata_rights**: Calculates the additional investment required for an investor to maintain their ownership percentage
- **calculate_basic_conversion**: Determines the core conversion metrics for a single SAFE instrument
- **compare_safe_versions**: Analyzes how different SAFE instrument terms affect the final outcome for the same investment
- **simulate_dilution_impact**: Evaluates how existing SAFE holders are diluted by new investors in a priced round


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAFE Conversion Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the conversion for a $500,000 SAFE with a $5,000,000 valuation cap and a 20% discount for a $10,000,000 next round."

**🤖 AI Agent:**
> The conversion price is $0.50 per share, resulting in 1,000,000 shares issued and an ownership stake of 5.0%.

---

**👤 You:**
> "How much should I invest to maintain 10% ownership if the current valuation is $2,000,000 and $500,000 is being raised?"

**🤖 AI Agent:**
> To maintain 10% ownership, the required investment is $55,555.56.

---

**👤 You:**
> "Compare a $100,000 investment with a $5M cap versus a 20% discount for a $10M next round valuation."

**🤖 AI Agent:**
> The $5M cap scenario results in a $0.50 conversion price and 200,000 shares, while the 20% discount scenario results in a $0.80 conversion price and 125,000 shares.


## ❓ FAQ

**Q: What is a SAFE?**
A SAFE is a financial instrument used by early-stage startups to raise capital, providing a contractual right to receive equity during a future priced financing round.

**Q: How does the tool handle different SAFE versions?**
The `calculate_basic_conversion` tool accepts a `safeType` parameter to account for different instrument versions like Standard_YC or Custom_Institutional.

**Q: Can I simulate how a new funding round affects my ownership?**
Yes, you can use the `simulate_dilution_impact` tool to evaluate how existing SAFE holders are diluted by new investors in a priced round.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/safe-conversion-engine](https://vinkius.com/en/ai-agent-connect/safe-conversion-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAFE Conversion Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `safe-conversion-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAFE Conversion Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "safe-conversion-engine": {
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
