# Dice Probability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dice-probability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate exact and simulated probabilities for any dice combination, including sums, face frequencies, and drop mechanics.

## Description
The Dice Probability Calculator is a powerful engine designed for tabletop gamers and statisticians. It provides precise probability distributions for various dice-rolling scenarios. Use `dice_sum_probability` to find the likelihood of achieving a specific sum, `face_frequency_probability` to track how often a certain face appears in a pool, or `modified_distribution_probability` to calculate outcomes when dropping the lowest dice (like in D&D 5e). The engine uses exact combinatorial math for pools up to 10 dice and switches to high-precision Monte Carlo simulation for larger pools to ensure speed and accuracy.


## Available Tools (3)
- **face_frequency_probability**: Calculate the probability of a specific face appearing in a pool of dice
- **modified_distribution_probability**: Calculate the probability of a dice sum after dropping lowest dice
- **dice_sum_probability**: Calculate the probability of a specific dice sum


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dice Probability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the probability of rolling a sum of at least 15 on 3d6?"

**🤖 AI Agent:**
> The probability of rolling a sum of at least 15 on 3d6 is approximately 0.0926 (9.26%).

---

**👤 You:**
> "How likely am I to roll at least one 6 when rolling 5d6?"

**🤖 AI Agent:**
> The probability of rolling at least one 6 on 5d6 is approximately 0.5981 (59.81%).

---

**👤 You:**
> "What's the chance of getting a sum of at least 12 on 4d6 after dropping the lowest die?"

**🤖 AI Agent:**
> The probability of rolling a sum of at least 12 on 4d6 after dropping the lowest die is approximately 0.8175 (81.75%).


## ❓ FAQ

**Q: How accurate are the results?**
For pools of 10 dice or fewer, the engine uses exact combinatorial logic for 100% precision. For larger pools, it utilizes Monte Carlo simulation, which provides a highly accurate estimate with negligible error.

**Q: Can I calculate probabilities for custom dice?**
Yes. You can specify any number of sides per die, allowing you to model standard dice like d6 or d20, as well as custom configurations.

**Q: Does it support mechanics like 'drop the lowest'?**
Yes, using the `modified_distribution_probability` tool, you can calculate the probability of a sum after removing the lowest N dice from your pool.


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
