# Sleep Consistency Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-consistency-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Quantify sleep regularity and circadian alignment through advanced stability analysis.

## Description
This MCP server provides a specialized analytical engine to quantify sleep regularity and circadian alignment. By analyzing bedtime and wake time patterns, it calculates a precise consistency score, measures social jetlag, and provides detailed variability metrics. Use `get_consistency_score` to find your stability rating, `get_social_jetlag_measure` to detect weekday vs. weekend misalignment, and `get_regularity_recommendations` for actionable advice to improve your sleep hygiene.


## Available Tools (4)
- **get_consistency_score**: Calculates a singular stability score for a given period of sleep data
- **get_regularity_recommendations**: Generates actionable advice based on calculated consistency and jetlag levels
- **get_social_jetlag_measure**: Measures the misalignment between weekday and weekend sleep patterns
- **get_variability_metrics**: Provides detailed statistical dispersion data for sleep timing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Consistency Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my sleep consistency score for these logs: [{"bedtime": "2023-10-01T22:00:00Z", "wakeTime": "2023-10-02T06:00:00Z"}, {"bedtime": "2023-10-02T22:15:00Z", "wakeTime": "2023-10-03T06:10:00Z"}]"

**🤖 AI Agent:**
> Your consistency score is 92, which is rated as Very High stability.

---

**👤 You:**
> "What is my social jetlag if my weekday bedtimes are 11 PM and my weekend bedtimes are 2 AM?"

**🤖 AI Agent:**
> Your social jetlag is 3.0 hours, indicating a moderate misalignment between your weekday and weekend rhythms.

---

**👤 You:**
> "Give me sleep recommendations for a consistency score of 45 and 4 hours of social jetlag."

**🤖 AI Agent:**
> To improve your regularity, try to reduce weekend sleep extension and maintain a more consistent bedtime throughout the week.


## ❓ FAQ

**Q: How do I calculate my sleep stability?**
You can use the `get_consistency_score` tool by providing a JSON array of your sleep logs containing bedtime and wake time timestamps.

**Q: What is social jetlag?**
Social jetlag is the discrepancy between your weekday sleep schedule and your weekend sleep schedule. The `get_social_jetlag_measure` tool quantifies this misalignment in hours.

**Q: Can I get advice to improve my sleep?**
Yes, the `get_regularity_recommendations` tool generates actionable suggestions based on your specific consistency score and social jetlag levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-consistency-index](https://vinkius.com/en/ai-agent-connect/sleep-consistency-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Consistency Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-consistency-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Consistency Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-consistency-index": {
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
