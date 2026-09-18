# Chronic Pain Diary Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/chronic-pain-diary-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Identifies correlations between physiological, environmental, and activity data to manage chronic pain.

## Description
This MCP server connects AI agents to your chronic pain history. It analyzes complex relationships between pain intensity, physical activities, sleep quality, and environmental factors like weather. By using tools like `get_pain_trends` and `identify_pain_triggers`, agents can detect patterns in your pain levels, find specific triggers, and even `predict_intervention_windows` to help you plan medication or therapy. It also uses `analyze_activity_sleep_correlation` to show how your lifestyle impacts your discomfort.


## Available Tools (4)
- **analyze_activity_sleep_correlation**: Analyzes the relationship between daily activities, sleep quality, and pain intensity
- **get_pain_trends**: Analyzes pain trends over a specified number of days
- **identify_pain_triggers**: Identifies significant factors that correlate with pain flares
- **predict_intervention_windows**: Predicts optimal windows for medication or therapeutic activities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chronic Pain Diary Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How has my pain been changing over the last 14 days?"

**🤖 AI Agent:**
> Your pain has been decreasing slightly, with an average intensity of 4.2 and low volatility over the last two weeks.

---

**👤 You:**
> "What are my main pain triggers?"

**🤖 AI Agent:**
> Your most significant triggers are high humidity and strenuous physical activity, which show a high correlation with your pain flares.

---

**👤 You:**
> "When is a good time for me to schedule my physical therapy this week?"

**🤖 AI Agent:**
> Based on your predicted low-pain windows, Thursday afternoon looks like an optimal time for your physical therapy.


## ❓ FAQ

**Q: How does the tool identify my pain triggers?**
The `identify_pain_triggers` tool analyzes historical logs to find statistical correlations between specific activities, weather changes, or biological markers and your reported pain scores.

**Q: Can I predict when my pain might flare up?**
Yes, by using `predict_intervention_windows`, the agent can identify periods of likely low pain or impending flares based on your historical weather sensitivity and menstrual cycle patterns.

**Q: Does it track how sleep affects my pain?**
Yes, the `analyze_activity_sleep_correlation` tool specifically evaluates how your sleep quality and physical activity levels influence your pain intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/chronic-pain-diary-analyzer](https://vinkius.com/en/ai-agent-connect/chronic-pain-diary-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chronic Pain Diary Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chronic-pain-diary-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chronic Pain Diary Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chronic-pain-diary-analyzer": {
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
