# One-Rep Max Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/one-rep-max-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Predict your maximum strength using multiple physiological models.

## Description
This MCP server provides precise strength forecasting by applying multiple mathematical models to your submaximal training data. Use `get_estimated_1rm` to calculate your predicted maximum weight based on the weight lifted, repetitions, and RPE. You can also use `get_percentage_tables` to generate training intensity charts, `get_formula_comparison` to evaluate model reliability, and `get_confidence_interval` to understand the statistical margin of error for your specific exercise type.


## Available Tools (4)
- **get_estimated_1rm**: Calculates the predicted 1RM using multiple mathematical models
- **get_confidence_interval**: Calculates the range within which the true 1RM likely falls
- **get_formula_comparison**: Provides a qualitative comparison of the different models to show which one is most reliable
- **get_percentage_tables**: Generates a breakdown of what various percentages of the estimated 1RM would look like in absolute weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **One-Rep Max Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just did 5 reps of 100kg bench press at RPE 8. What is my estimated 1RM?"

**🤖 AI Agent:**
> Your estimated 1RM for bench press is 120kg.

---

**👤 You:**
> "Show me a percentage table for a 200kg squat."

**🤖 AI Agent:**
> For a 200kg squat, your training weights are: 50%: 100kg, 60%: 120kg, 70%: 140kg, 75%: 150kg, 80%: 160kg, 85%: 170kg, 90%: 180kg, 95%: 190kg.

---

**👤 You:**
> "How much error should I expect for a 3 rep set of 150kg deadlift?"

**🤖 AI Agent:**
> The estimated 1RM is 165kg with a confidence interval of 158kg to 172kg.


## ❓ FAQ

**Q: How accurate are these 1RM estimates?**
Accuracy depends on the number of repetitions performed. You can use `get_confidence_interval` to see the calculated margin of error for your specific set.

**Q: Which formula is best for my training?**
Different models excel at different rep ranges. Use `get_formula_comparison` to see which model is recommended for your specific number of repetitions.

**Q: Can I include RPE in my calculation?**
Yes, providing your Rate of Perceived Exertion (RPE) to `get_estimated_1rm` allows the tool to adjust for reps in reserve, leading to a more personalized estimate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/one-rep-max-estimator](https://vinkius.com/en/ai-agent-connect/one-rep-max-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **One-Rep Max Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `one-rep-max-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **One-Rep Max Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "one-rep-max-estimator": {
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
