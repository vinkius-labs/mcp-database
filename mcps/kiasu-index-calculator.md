# Kiasu Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kiasu-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Quantify Kiasu behavior intensity with deterministic scoring.

## Description
This MCP server provides tools to measure the intensity of 'Kiasu' behaviors. Use `calculate_kiasu_index` to determine a user's Kiasu level (Casual, Dedicated, or Legendary) based on specific behavioral weights. You can also use `get_behavior_weights` to inspect individual weights or `get_kiasu_classification_ranges` to see the scoring thresholds.


## Available Tools (3)
- **calculate_kiasu_index**: 
- **get_behavior_weights**: 
- **get_kiasu_classification_ranges**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kiasu Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my Kiasu index for these behaviors: queue_for_freebie, bring_own_bag, compare_grades."

**🤖 AI Agent:**
> Your total Kiasu score is 60, which puts you in the Dedicated level. Your top behaviors were compare_grades, queue_for_freebie, and bring_own_bag.

---

**👤 You:**
> "What is the weight for the behavior 'take_extra_napkins'?"

**🤖 AI Agent:**
> The weight for 'take_extra_napkins' is 15.

---

**👤 You:**
> "Check my Kiasu level if I queue_for_freebie and avoid_risky_food."

**🤖 AI Agent:**
> Your total Kiasu score is 20, making you a Casual level. Your Kiasi score is 10.


## ❓ FAQ

**Q: How is the Kiasu score calculated?**
The score is a sum of fixed weights assigned to specific behaviors like `queue_for_freebie` or `compare_grades`.

**Q: What is the Kiasi score?**
The Kiasi score is a secondary metric that increases if the `avoid_risky_food` behavior is detected.

**Q: What are the Kiasu levels?**
Levels are classified as Casual (0-30), Dedicated (31-60), or Legendary (61-100).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kiasu-index-calculator](https://vinkius.com/ai-agent-connect/kiasu-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kiasu Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kiasu-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kiasu Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kiasu-index-calculator": {
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
