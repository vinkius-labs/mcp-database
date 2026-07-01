# Progressive Overload Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/progressive-overload-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Automate 12-week strength training schedules with safety-capped linear progression.

## Description
The Progressive Overload Planner is a specialized tool for lifters seeking to maximize strength gains while protecting connective tissue. By using the `compute_training_schedule` tool, you can generate a precise 12-week weight progression based on your starting load and desired weekly increments. The system automatically applies safety caps via the `validate_increment_safety` logic to ensure that no single week's jump exceeds your specified percentage threshold, preventing tendon strain. Additionally, use `predict_progression_plateau` to identify exactly when your training intensity might hit a structural limit based on your current parameters.


## Available Tools (3)
- **compute_training_schedule**: Generates a complete 12-week spreadsheet of target weights for a lifting program
- **predict_progression_plateau**: Estimates at which week in a 12-week cycle the safety cap will first be triggered
- **validate_increment_safety**: Checks whether a proposed weight increase adheres to safety constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Progressive Overload Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 12-week training schedule starting at 60kg, adding 2.5kg each week, with a maximum jump of 5%."

**🤖 AI Agent:**
> Week 1: 60kg, Week 2: 62.5kg, Week 3: 65kg, Week 4: 67.5kg, Week 5: 70kg, Week 6: 72.5kg, Week 7: 75kg, Week 8: 77.5kg, Week 9: 80kg, Week 10: 82.5kg, Week 11: 85kg, Week 12: 87.5kg.

---

**👤 You:**
> "Is it safe to jump from 100kg to 110kg if my max jump percent is set to 8%?"

**🤖 AI Agent:**
> No, that jump represents a 10% increase. The suggested weight to stay within your 8% limit would be 108kg.

---

**👤 You:**
> "When will I hit my safety cap if I start at 50kg and add 5kg weekly with a 10% max jump?"

**🤖 AI Agent:**
> The safety cap will first be triggered in Week 3.


## ❓ FAQ

**Q: How does the safety cap work?**
The planner monitors the percentage increase between weeks. If a scheduled increment would cause a jump larger than your `maxJumpPercent`, the tool automatically caps the weight at the maximum safe threshold to prevent injury.

**Q: Can I use this for different training styles?**
While optimized for linear progression, you can adapt it by adjusting the `weeklyIncrementKg` and `maxJumpPercent` to match your specific methodology.

**Q: What does the plateau prediction tell me?**
The `predict_progression_plateau` tool simulates your entire 12-week cycle and identifies the specific week where your weight increases will first trigger the safety cap.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/progressive-overload-planner](https://vinkius.com/mcp/progressive-overload-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Progressive Overload Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `progressive-overload-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Progressive Overload Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "progressive-overload-planner": {
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
