# Sleep Diary Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-diary-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyzes sleep diary entries to identify patterns, red flags, and clinical insights.

## Description
This MCP server connects AI agents to detailed sleep data analysis. It processes sleep diary entries to calculate key metrics like sleep efficiency and consistency. Use `analyze_sleep_summary` for high-level metric overviews, `detect_sleep_patterns` to find trends like decreasing duration, `identify_red_flags` to spot physiological risks, and `generate_clinical_insights` for qualitative observations based on sleep architecture.


## Available Tools (4)
- **analyze_sleep_summary**: Provides a high-level overview of sleep metrics for a specific period
- **detect_sleep_patterns**: Requires at least three entries to establish a trend.

Identifies recurring trends such as progressive sleep loss or rhythmic disturbances
- **generate_clinical_insights**: Translates raw metrics into qualitative observations for professional or personal review
- **identify_red_flags**: Flags specific metrics that fall outside of healthy physiological ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Diary Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you summarize my sleep metrics for the last week?"

**🤖 AI Agent:**
> Your average sleep duration was 7.2 hours with a sleep efficiency of 88% and an average latency of 15 minutes.

---

**👤 You:**
> "Are there any concerning trends in my sleep lately?"

**🤖 AI Agent:**
> Yes, there is a pattern of increasing_latency over the last four days, suggesting it is taking longer to fall asleep.

---

**👤 You:**
> "Check if there are any red flags in my sleep data."

**🤖 AI Agent:**
> A high impact fragmentation_risk was detected due to frequent nocturnal awakenings recorded in your recent entries.


## ❓ FAQ

**Q: What kind of data does this server process?**
It processes sleep diary entries including bedtime, wake time, sleep onset latency, number of awakenings, and subjective sleep quality.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this MCP server to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.

**Q: Does this provide medical diagnoses?**
No. The tool provides observations of data patterns and identifies potential red flags for review, but it does not provide medical diagnoses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-diary-analyzer](https://vinkius.com/en/ai-agent-connect/sleep-diary-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Diary Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-diary-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Diary Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-diary-analyzer": {
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
