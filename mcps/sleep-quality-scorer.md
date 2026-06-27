# Sleep Quality Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sleep-quality-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze your sleep patterns and receive a diagnostic score based on duration, continuity, and subjective recovery.

## Description
The Sleep Quality Scorer MCP connects AI agents to your nocturnal metrics. By using tools like `calculate_overall_quality`, `assess_sleep_duration`, `evaluate_sleep_continuity`, and `diagnose_morning_subjectivity`, the agent can evaluate how hours slept, awakenings, and waking feelings impact your overall sleep architecture and health recommendations.


## Available Tools (4)
- **diagnose_morning_subjectivity**: Diagnose morning subjectivity
- **assess_sleep_duration**: Assess sleep duration quality
- **calculate_overall_quality**: Calculate overall sleep quality score
- **evaluate_sleep_continuity**: Evaluate sleep continuity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Quality Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I slept for 7.5 hours, woke up 1 time, and I feel rested. What is my sleep quality score?"

**🤖 AI Agent:**
> Your overall sleep quality score is high because your duration was optimal and you experienced minimal disruption.

---

**👤 You:**
> "I slept for 5 hours, woke up 4 times, and I feel exhausted. Analyze my sleep."

**🤖 AI Agent:**
> Your sleep quality is low due to insufficient duration and high fragmentation from frequent awakenings.

---

**👤 You:**
> "Check if 8 hours of sleep is considered optimal for me."

**🤖 AI Agent:**
> 8 hours of sleep falls within the optimal tier, providing a great foundation for recovery.


## ❓ FAQ

**Q: How is the sleep quality score calculated?**
The score is a composite value derived from your total hours slept, the number of times you woke up during the night, and how rested you feel upon waking.

**Q: Can I analyze specific aspects like sleep duration?**
Yes, you can use `assess_sleep_duration` to see if your sleep was optimal, deprived, or excessive.

**Q: What happens if I report many awakenings?**
Using `evaluate_sleep_continuity` will show a higher disruption level and a lower continuity score as the number of interruptions increases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sleep-quality-scorer](https://vinkius.com/mcp/sleep-quality-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Quality Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-quality-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Quality Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-quality-scorer": {
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
