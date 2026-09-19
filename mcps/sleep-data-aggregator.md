# Sleep Data Aggregator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sleep-data-aggregator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Unify sleep metrics from trackers, diaries, and subjective ratings.

## Description
This MCP connects AI agents to your sleep data ecosystem. It aggregates information from wearable trackers, manual diary entries, and subjective wellness ratings to provide a single source of truth. Use `get_unified_metrics` to see a combined view of sleep duration and efficiency, `detect_sleep_discrepancies` to find mismatches between hardware data and user reports, and `get_confidence_analysis` to understand the statistical certainty of your sleep metrics.


## Available Tools (4)
- **detect_sleep_discrepancies**: Identifies significant conflicts between objective tracker measurements and subjective user reports
- **aggregate_source_summary**: Provides a breakdown of how much data is being contributed by each specific source
- **get_confidence_analysis**: Calculates the statistical certainty of the current sleep data set
- **get_unified_metrics**: Provides a single, coherent view of sleep metrics by combining all available data sources


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Data Aggregator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my total sleep duration and efficiency for the last week?"

**🤖 AI Agent:**
> Your total sleep duration for the last week was 48.5 hours with an average sleep efficiency of 88%.

---

**👤 You:**
> "Are there any mismatches between my tracker and my diary?"

**🤖 AI Agent:**
> Yes, there were 2 significant conflicts where your tracker reported longer sleep than your manual diary entries.

---

**👤 You:**
> "How certain is my sleep efficiency data?"

**🤖 AI Agent:**
> The current confidence level for your sleep efficiency is high, with a narrow confidence interval due to consistent tracker and diary agreement.


## ❓ FAQ

**Q: How does this tool handle different data sources?**
The tool uses weighted averages to combine tracker data and manual diary entries, prioritizing high-frequency tracker data for precise timing.

**Q: What is a sleep discrepancy?**
A discrepancy occurs when there is a significant difference between what your wearable tracker reports and what you record in your sleep diary.

**Q: Can I see how complete my sleep data is?**
Yes, you can use `aggregate_source_summary` to view the data completeness percentage across tracker, diary, and subjective sources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sleep-data-aggregator](https://vinkius.com/en/ai-agent-connect/sleep-data-aggregator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Data Aggregator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-data-aggregator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Data Aggregator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-data-aggregator": {
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
