# Wine Tannin Addition Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-tannin-addition-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Calculate precise tannin additions for wine structure and mouthfeel.

## Description
This MCP server provides enologists with precise tools to manage tannin levels in wine. Use `calculate_addition_requirement` to determine the exact mass of additives needed based on current ppm and target levels. The `predict_sensory_impact` tool estimates changes in mouthfeel and astringency by accounting for tannin type and protein binding. Additionally, `evaluate_threshold_safety` checks if additions stay within sensory limits, while `generate_bench_trial_protocol` provides laboratory testing steps for small-scale validation.


## Available Tools (4)
- **calculate_addition_requirement**: Determines the exact mass of a specific tannin product needed to reach a desired target concentration
- **evaluate_threshold_safety**: Validates whether the proposed addition will likely exceed or fall below sensory detection limits
- **generate_bench_trial_protocol**: Recommends a small-scale laboratory testing procedure based on the calculated addition
- **predict_sensory_impact**: Estimates how the planned tannin addition will change the wine's mouthfeel and perceived astringency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Tannin Addition Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 1000L of wine with 50ppm tannin. I want to reach 80ppm using a product that is 50% pure tannin. How much should I add?"

**🤖 AI Agent:**
> You need to add 60 grams of the tannin product to reach the target of 80ppm in 1000L of wine.

---

**👤 You:**
> "What will be the sensory impact of adding 20ppm of proanthocyanidins to a wine with 10ppm current tannin and 50ppm protein level?"

**🤖 AI Agent:**
> The addition will result in a moderate impact, providing noticeable structural enhancement with a moderate increase in perceived astringency.

---

**👤 You:**
> "Is it safe to add 15ppm of ellagitannins if my current level is 40ppm?"

**🤖 AI Agent:**
> Yes, the addition is within the sensory threshold for ellagitannins and is unlikely to cause unexpected sensory shifts.


## ❓ FAQ

**Q: How do I calculate the amount of tannin to add?**
Use the `calculate_addition_requirement` tool by providing the current tannin level, target level, wine volume, and the purity of your additive.

**Q: Can I predict how the wine's mouthfeel will change?**
Yes, the `predict_sensory_impact` tool estimates changes in astringency and mouthfeel based on the tannin type and protein concentration.

**Q: Should I perform a bench trial before full production?**
It is highly recommended. You can use `generate_bench_trial_protocol` to get a specific laboratory procedure for testing your addition.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-tannin-addition-calculator](https://vinkius.com/en/ai-agent-connect/wine-tannin-addition-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Tannin Addition Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-tannin-addition-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Tannin Addition Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-tannin-addition-calculator": {
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
