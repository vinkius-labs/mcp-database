# Loyalty Points Value Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/loyalty-points-value-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the economic value of loyalty points, redemption efficiency, and expiration risks.

## Description
This MCP server provides tools to accurately determine the monetary value of loyalty programs. Use `calculate_point_worth` to find the value of a single point, `analyze_redemption_efficiency` to compare different reward options, `evaluate_expiry_impact` to assess the financial risk of expiring points, and `calculate_net_redemption_cost` to determine the final out-of-pocket expense when using points for purchases.


## Available Tools (4)
- **calculate_net_redemption_cost**: Calculates the actual out-of-pocket cost for a user using points to offset a purchase
- **calculate_point_worth**: Calculates the monetary value of a single loyalty point and the cost to earn it
- **evaluate_expiry_impact**: Calculates the effective loss of value due to point expiration
- **analyze_redemption_efficiency**: Each option should be an object with rewardValue, pointsCost, and transactionFee.

Determines which redemption method provides the best value for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loyalty Points Value Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much is one point worth if I spend $100 to earn 50 points, and those 50 points can be used for a $10 reward?"

**🤖 AI Agent:**
> One point is worth $0.20, and the earning rate is $2.00 per point.

---

**👤 You:**
> "I have 1000 points worth $0.10 each, and 200 points are expiring soon. What is my risk?"

**🤖 AI Agent:**
> The total value at risk is $20.00, which represents 20% of your total balance.

---

**👤 You:**
> "What is the net cost of a $50 item if I use points worth $30 and there is a $5 redemption fee?"

**🤖 AI Agent:**
> The net cash required is $25.00, and the total effective cost is $55.00.


## ❓ FAQ

**Q: How do I know if a redemption option is a good deal?**
You can use the `analyze_redemption_efficiency` tool. It compares different reward options by calculating the ratio of reward value (minus fees) to the points cost, identifying the most efficient path.

**Q: Can I calculate the risk of my points expiring?**
Yes, the `evaluate_expiry_impact` tool calculates the total monetary value at risk and the percentage of your balance that is set to expire.

**Q: How much is one loyalty point worth in cash?**
The `calculate_point_worth` tool determines the specific monetary value of a single point based on the purchase price, points earned, and the value of the reward received.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/loyalty-points-value-calculator](https://vinkius.com/en/ai-agent-connect/loyalty-points-value-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loyalty Points Value Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `loyalty-points-value-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loyalty Points Value Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loyalty-points-value-calculator": {
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
