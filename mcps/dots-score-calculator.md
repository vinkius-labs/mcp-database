# DOTS Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dots-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate modern DOTS scores and strength levels for powerlifting.

## Description
This MCP server provides a specialized toolset for powerlifters to evaluate their performance. It allows users to calculate their modern DOTS score, compare it against the historical Wilks standard, and determine their strength level (Novice, Intermediate, Advanced, or Elite). Use `calculate_dots_score` to get the primary coefficient, `compare_to_wilks` to see how modern standards differ from historical ones, and `get_strength_level` to classify performance.


## Available Tools (4)
- **compare_to_wilks**: Compares the lifter's DOTS performance against the historical Wilks standard
- **evaluate_relative_strength**: Provides a qualitative assessment of strength relative to the athlete's weight
- **get_strength_level**: Classifies the athlete into a strength category based on their DOTS score
- **calculate_dots_score**: Calculates the primary DOTS coefficient for a lifter


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DOTS Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my DOTS score. I am a male, I weigh 90kg, and my total lift is 500kg."

**🤖 AI Agent:**
> Your DOTS score is 415.2.

---

**👤 You:**
> "What is my strength level if my DOTS score is 350?"

**🤖 AI Agent:**
> A DOTS score of 350 classifies you as an Intermediate lifter.

---

**👤 You:**
> "Compare my performance to Wilks. I am a female, weigh 65kg, and lifted 300kg."

**🤖 AI Agent:**
> Your Wilks score is 285.5, showing a difference of 12.3 from your DOTS score.


## ❓ FAQ

**Q: What is a DOTS score?**
A DOTS score is a modern relative strength coefficient used in powerlifting to compare lifters of different body weights and genders.

**Q: How do I know my strength level?**
You can use the `get_strength_level` tool after calculating your DOTS score to see if you are Novice, Intermediate, Advanced, or Elite.

**Q: Can I compare DOTS to Wilks?**
Yes, the `compare_to_wilks` tool allows you to see the mathematical difference between modern DOTS and the historical Wilks standard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dots-score-calculator](https://vinkius.com/en/ai-agent-connect/dots-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DOTS Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dots-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DOTS Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dots-score-calculator": {
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
