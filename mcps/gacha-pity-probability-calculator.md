# Gacha Pity Probability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gacha-pity-probability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Simulate gacha pity mechanics and analyze monetization impact.

## Description
A deterministic modeling engine for game designers to simulate gacha monetization and player spending behavior. Use `calculate_pity_dynamics` to model step-by-step probability mechanics, including base rates, soft pity ramps, and hard pity guarantees. Once the dynamics are modeled, use `analyze_monetization_impact` to calculate expected costs and identify design risks like predatory mechanics. You can also use `get_pity_summary` to quickly extract statistical central tendencies like median pulls and the most likely pull number.


## Available Tools (3)
- **analyze_monetization_impact**: Converts pity simulation data into financial and design-risk metrics
- **get_pity_summary**: Provides a high-level summary of the system feel and statistical central tendencies
- **calculate_pity_dynamics**: Simulates the step-by-step probability mechanics of a gacha system


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gacha Pity Probability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dynamics for a gacha with a 1% base rate, soft pity starting at pull 50 with a 2% increase per pull, and hard pity at 80 pulls. Simulate 100 pulls."

**🤖 AI Agent:**
> The simulation for your gacha system shows an expected number of pulls of 54.2 and a whale probability of 0.12. The probability per pull increases steadily from pull 50 until it reaches 100% at pull 80.

---

**👤 You:**
> "Analyze the monetization impact for a system where the expected pulls is 65 and the cost per pull is 2.50 units."

**🤖 AI Agent:**
> The average cost per obtain is 162.50 units. The estimated revenue per player is also 162.50 units based on the expected pulls.

---

**👤 You:**
> "Give me a summary of the pity dynamics for a system with a 0.5% base rate and hard pity at 90."

**🤖 AI Agent:**
> The median number of pulls to obtain the item is 72, and the most likely pull is 75. The total success chance at the end of the simulation is 100%.


## ❓ FAQ

**Q: How do I model a soft pity system?**
Use the `calculate_pity_dynamics` tool. Set the `baseRatePercent`, define when the increase starts with `softPityStartPull`, and specify the increment with `softPityRateIncreasePerPull`.

**Q: Can I check if my gacha system is too predatory?**
Yes. After running `calculate_pity_dynamics`, pass the result to `analyze_monetization_impact`. It will return a `designFlags` object containing an `isPredatory` flag if the whale probability is too high.

**Q: What is the difference between soft pity and hard pity?**
Soft pity is a gradual increase in success probability after a certain number of pulls. Hard pity is the specific pull number where the success probability becomes 100%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gacha-pity-probability-calculator](https://vinkius.com/ai-agent-connect/gacha-pity-probability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gacha Pity Probability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gacha-pity-probability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gacha Pity Probability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gacha-pity-probability-calculator": {
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
