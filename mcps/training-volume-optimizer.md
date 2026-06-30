# Training Volume Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/training-volume-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate optimal weekly training sets (MEV, MAV, MRV) and session distribution based on hypertrophy principles.

## Description
The Training Volume Optimizer is a physiological calculation engine designed to determine the ideal amount of training volume for your goals. Using established principles of stimulus vs. fatigue, it calculates three critical thresholds: MEV (Minimum Effective Volume), MAV (Maximum Adaptive Volume), and MRV (Maximum Recoverable Volume). By using tools like `get_volume_bounds`, you can find the specific set ranges for any muscle group based on your experience level and training goal. Additionally, use `distribute_sets_per_session` to split your weekly volume across training days and `validate_training_load` to ensure you are not underperforming or overreaching.


## Available Tools (3)
- **distribute_sets_per_session**: Calculates how to split weekly sets across training days
- **get_volume_bounds**: Calculates MEV, MAV, and MRV thresholds
- **validate_training_load**: Checks if current volume poses a risk of overtraining or underperformance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Training Volume Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the optimal weekly sets for Chest if I am an Intermediate lifter focused on Hypertrophy?"

**🤖 AI Agent:**
> For Chest at an Intermediate level with a Hypertrophy goal, your MEV is 10 sets, MAV is 14 sets, and MRV is 20 sets per week.

---

**👤 You:**
> "How should I distribute 15 weekly sets for Back if I train it 3 times a week?"

**🤖 AI Agent:**
> You should perform 5 sets per session, with 0 residual sets.

---

**👤 You:**
> "I am doing 25 sets for Quads, but my MRV is 20. Am I okay?"

**🤖 AI Agent:**
> No, your status is Overreaching with a High risk level because you have exceeded your MRV.


## ❓ FAQ

**Q: What are MEV, MAV, and MRV?**
MEV is the minimum volume needed for progress. MAV is the optimal range for growth. MRV is the maximum volume you can recover from.

**Q: How do I use `get_volume_bounds`?**
Provide the muscle group, your training goal (Hypertrophy, Strength, or Endurance), and your experience level to get your weekly set ranges.

**Q: Can I check if I am overtraining?**
Yes, use the `validate_training_load` tool by inputting your current weekly volume along with your MEV and MRV thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/training-volume-optimizer](https://vinkius.com/mcp/training-volume-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Training Volume Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `training-volume-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Training Volume Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "training-volume-optimizer": {
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
