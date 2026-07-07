# Drop Set Percentage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drop-set-percentage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Calculate exact weight reductions for consecutive drop sets.

## Description
This MCP server provides specialized tools for strength athletes to calculate the precise weight sequence required for multi-stage drop sets. Using `generate_drop_sequence`, you can determine every weight that should be loaded on the bar based on a fixed percentage reduction. The `calculate_drop_summary` tool helps assess the total workload impact, while `evaluate_drop_intensity` categorizes your training strategy into shallow, moderate, or aggressive intensity tiers.


## Available Tools (3)
- **evaluate_drop_intensity**: Categorizes the difficulty of a drop set strategy
- **generate_drop_sequence**: Generates a sequence of weights for consecutive drop sets
- **calculate_drop_summary**: Calculates the impact of drops on total workload


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drop Set Percentage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm starting a drop set at 100kg with 3 drops and a 20% reduction. What weights should I use?"

**🤖 AI Agent:**
> Your weight sequence for the drops will be: 80.0kg, 64.0kg, and 51.2kg.

---

**👤 You:**
> "If I reduce the weight by 30% for 2 drops starting from 60kg, how much total weight is removed?"

**🤖 AI Agent:**
> The total weight removed throughout the sequence is 31.4kg.

---

**👤 You:**
> "Is a 40% reduction considered an aggressive drop set?"

**🤖 AI Agent:**
> Yes, a 40% reduction is categorized as an aggressive intensity tier.


## ❓ FAQ

**Q: How does the weight reduction calculation work?**
The tool calculates each subsequent drop based on the weight currently on the bar. For example, if you start at 100kg with a 20% reduction, the first drop will be 80kg, and the second drop will be 64kg.

**Q: What does `evaluate_drop_intensity` tell me?**
It categorizes your reduction percentage into three tiers: shallow, moderate, or aggressive, helping you plan for metabolic stress versus mechanical tension.

**Q: Can I use this for any weightlifting discipline?**
Yes, it is designed for any athlete using drop set techniques in resistance training to maintain consistent intensity across reductions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drop-set-percentage-calculator](https://vinkius.com/mcp/drop-set-percentage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drop Set Percentage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drop-set-percentage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drop Set Percentage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drop-set-percentage-calculator": {
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
