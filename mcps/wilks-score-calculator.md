# Wilks Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wilks-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate relative strength using Wilks coefficients.

## Description
This MCP server provides specialized tools for powerlifting athletes to determine their relative strength. By using the `calculate_wilks_score` tool, lifters can normalize their total weight lifted against their body weight and gender. The server also includes tools to `compare_to_records` for performance tiering and `get_relative_strength_ranking` to categorize strength profiles.


## Available Tools (4)
- **calculate_wilks_score**: Calculates the Wilks score and coefficient for a lifter
- **compare_to_records**: Evaluates how the athlete's score compares to established strength milestones
- **get_formula_metadata**: Provides technical details about the specific version of the Wilks formula being applied
- **get_relative_strength_ranking**: Provides a qualitative assessment of the athlete's strength profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wilks Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my Wilks score. I weigh 85kg, I am male, and my total lift is 500kg."

**🤖 AI Agent:**
> Your Wilks score is 412.5.

---

**👤 You:**
> "What is my strength category for a 60kg female lifter with a 250kg total?"

**🤖 AI Agent:**
> You are categorized as an Advanced lifter.

---

**👤 You:**
> "Compare a Wilks score of 450 for a male lifter to the records."

**🤖 AI Agent:**
> A score of 450 places you in the Elite tier.


## ❓ FAQ

**Q: What is a Wilks score?**
A Wilks score is a value used to compare the strength of lifters with different body weights and genders.

**Q: Can I use the Wilks-2 formula?**
Yes, you can specify the use of the improved Wilks-2 coefficients within the `calculate_wilks_score` tool.

**Q: How do I know my strength tier?**
You can use the `compare_to_records` tool after calculating your score to see if you fall into the Novice, Intermediate, Advanced, Elite, or World Class category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wilks-score-calculator](https://vinkius.com/en/ai-agent-connect/wilks-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wilks Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wilks-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wilks Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wilks-score-calculator": {
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
