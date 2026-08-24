# Yarn Substitution Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/yarn-substitution-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate exact yarn requirements and fiber compatibility for knitting and crochet substitutions.

## Description
This MCP server provides precise tools for knitters and crocheters to swap yarns safely. Use `get_substitution_requirements` to determine the exact grams and skeins needed when changing yarn weight or gauge. Use `analyze_fiber_compatibility` to check if different materials like wool and cotton will behave similarly in your project. You can also use `get_gauge_impact_summary` to understand how a change in gauge will physically alter the dimensions of your finished piece.


## Available Tools (3)
- **analyze_fiber_compatibility**: Analyze fiber compatibility
- **get_gauge_impact_summary**: Summarize gauge impact
- **get_substitution_requirements**: Calculate substitute yarn requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yarn Substitution Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to substitute a worsted weight wool yarn (100g, 200m/g) with a bulky acrylic yarn (50g, 100m/g). The pattern needs 500m. The gauge difference is 15%. How much do I need?"

**🤖 AI Agent:**
> You will need 575 grams of the bulky acrylic yarn, which equals 12 skeins based on the 50g weight.

---

**👤 You:**
> "Is it okay to use silk instead of alpaca for this sweater?"

**🤖 AI Agent:**
> The compatibility score is 85. While both have good drape, silk has significantly less elasticity than alpaca, which may cause the sweater to stretch out over time.

---

**👤 You:**
> "How much will my project change if my gauge is 10% thicker than the pattern?"

**🤖 AI Agent:**
> A 10% thicker gauge will result in a smaller project if you do not adjust your yardage. You should apply a 1.10 multiplier to your required meters.


## ❓ FAQ

**Q: How do I know if my substitute yarn is the right amount?**
You can use the `get_substitution_requirements` tool. By providing the original yarn specs and the substitute yarn specs, it calculates the exact grams and skeins required.

**Q: Can I substitute cotton for wool?**
To check this, use `analyze_fiber_compatibility`. It will provide a compatibility score and a warning if the lack of elasticity in cotton might affect your project's drape.

**Q: What happens if my gauge is different?**
The `get_gauge_impact_summary` tool explains how the gauge difference will change the size of your project and provides a multiplier to adjust your yardage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/yarn-substitution-calculator](https://vinkius.com/ai-agent-connect/yarn-substitution-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yarn Substitution Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yarn-substitution-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yarn Substitution Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yarn-substitution-calculator": {
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
