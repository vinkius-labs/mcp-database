# Early Breaking Decision Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/early-breaking-decision-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Quantify the metabolic cost of breaking a fast before your target duration.

## Description
The Early Breaking Decision Engine provides a precise evaluation of the physiological opportunity cost incurred when terminating a fasting period prematurely. By analyzing your `targetHours` and `actualHoursAchieved`, the engine calculates your progress and estimates the metabolic loss, specifically focusing on the 14-hour autophagy threshold. Use `fasting_progress_tool` to see your completion percentage and `metabolic_loss_tool` to understand the impact on fat-burning potential.


## Available Tools (2)
- **metabolic_loss_tool**: Estimate the metabolic loss magnitude from breaking a fast early
- **fasting_progress_tool**: Calculate the percentage of a fasting window completed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Early Breaking Decision Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I planned to fast for 18 hours but I've only done 10. How much progress have I made and what is the metabolic cost?"

**🤖 AI Agent:**
> You completed 55.5% of your fast. Breaking now results in a 100% metabolic loss because you have not yet reached the 14-hour autophagy threshold.

---

**👤 You:**
> "I've fasted for 16 hours out of a 20 hour goal. What is my progress?"

**🤖 AI Agent:**
> You completed 80% of your fasting window.

---

**👤 You:**
> "Check my metabolic loss for a 24 hour fast where I've achieved 15 hours."

**🤖 AI Agent:**
> Your metabolic loss magnitude is approximately 37.5% as you have passed the initial autophagy threshold.


## ❓ FAQ

**Q: What is the 14-hour threshold?**
The 14-hour mark is a critical biological milestone where significant cellular cleanup processes, known as autophagy, are likely to begin.

**Q: How does the engine calculate metabolic loss?**
If you break your fast before 14 hours, the loss is considered 100%. After 14 hours, the cost decreases linearly as you approach your target duration.

**Q: Can I use this to track my fasting progress?**
Yes, by using the `fasting_progress_tool`, you can see exactly what percentage of your planned fasting window you have successfully completed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/early-breaking-decision-engine](https://vinkius.com/mcp/early-breaking-decision-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Early Breaking Decision Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `early-breaking-decision-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Early Breaking Decision Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "early-breaking-decision-engine": {
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
