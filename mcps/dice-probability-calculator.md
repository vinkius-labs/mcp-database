# Dice Probability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dice-probability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate full probability distributions, statistical metrics, and success thresholds for any dice notation.

## Description
The Dice Probability Calculator is a specialized engine designed to model the mathematical outcomes of tabletop gaming dice rolls. By providing specific dice notations like '2d6' or '1d20+5', users can instantly retrieve complete statistical profiles including mean, median, mode, and standard deviation. The tool supports advanced mechanics such as advantage, disadvantage, and dropping lowest dice (e. handles 4d6 drop lowest). Use `compute_dice_distribution` to see the full frequency distribution, `calculate_threshold_probability` to find your chance of hitting a specific Difficulty Class (DC), or `compare_roll_mechanics` to quantify exactly how much advantage improves your success rate against a target value.


## Available Tools (3)
- **compare_roll_mechanics**: Quantifies the impact of changing a roll mechanic
- **compute_dice_distribution**: g., "1d6"). Supports modifiers, dropCount, and mechanics like advantage/disadvantage.

Computes the statistical profile for a dice notation
- **calculate_threshold_probability**: Determines the probability of achieving a result >= target value


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dice Probability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the average roll and standard deviation for 2d6?"

**🤖 AI Agent:**
> For a 2d6 roll, the mean (average) is 7.0 and the standard deviation is approximately 1.71.

---

**👤 You:**
> "What is my chance of rolling a 15 or higher on a 1d20+5?"

**🤖 AI Agent:**
> The probability of achieving a result of 15 or higher with 1d20+5 is 35%.

---

**👤 You:**
> "How much does advantage improve my chance of hitting a DC 15 on a 1d20 roll?"

**🤖 AI Agent:**
> Switching from a straight roll to advantage increases your success probability against DC 15 from 30% to 51.25%, an improvement of 21.25%.


## ❓ FAQ

**Q: What dice notations are supported?**
The engine supports standard notation like '1d20', '2d6+3', and complex rules like '4d6' with the `dropCount` parameter to simulate dropping the lowest die.

**Q: How can I calculate my chance of success against a specific DC?**
Use the `calculate_threshold_probability` tool. Provide your dice notation and the target value (DC) to get the exact percentage chance of success.

**Q: Can I compare advantage vs. disadvantage?**
Yes, the `compare_roll_mechanics` tool allows you to compare a base roll against 'advantage' or 'disadvantage' using metrics like mean or threshold success.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dice-probability-calculator](https://vinkius.com/mcp/dice-probability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dice Probability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dice-probability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dice Probability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dice-probability-calculator": {
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
