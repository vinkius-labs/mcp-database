# Gratitude Journal Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gratitude-journal-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze gratitude patterns, consistency, and wellbeing correlations.

## Description
This MCP server provides deep analytical insights into gratitude journaling practices. It allows AI agents to process journal entries to identify recurring themes, measure how consistently a user journals, and evaluate the emotional depth of entries. By using tools like `analyze_theme_distribution` and `get_wellbeing_correlation`, agents can uncover how regular practice relates to emotional wellbeing and identify specific areas of life that trigger the most gratitude.


## Available Tools (4)
- **analyze_theme_distribution**: Identify which subjects or categories the user is most frequently grateful for
- **calculate_consistency_metrics**: Measure the regularity and habit strength of the gratitude practice
- **evaluate_entry_quality**: Assess the depth and emotional resonance of specific journal entries
- **get_wellbeing_correlation**: Determine if the user's gratitude practice is translating into measurable emotional patterns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gratitude Journal Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Based on my recent journal entries, what are my most common gratitude themes?"

**🤖 AI Agent:**
> Your primary theme is 'Family', appearing in 60% of your entries, followed by 'Nature' at 25%.

---

**👤 You:**
> "How consistent has my gratitude practice been lately?"

**🤖 AI Agent:**
> Your current consistency score is 85, with a current streak of 5 days and an average gap of 1.2 days between entries.

---

**👤 You:**
> "Is there a link between how often I journal and my emotional sentiment?"

**🤖 AI Agent:**
> Yes, there is a positive correlation between your journaling frequency and sentiment, suggesting that more regular practice leads to higher emotional resonance.


## ❓ FAQ

**Q: What kind of data does this tool analyze?**
The tool analyzes journal entries containing text, timestamps, and associated themes to provide insights into consistency and sentiment.

**Q: How can I check my journaling consistency?**
You can use the `calculate_consistency_metrics` tool to receive a consistency score, current streak, and average gap between entries.

**Q: Can it identify my most frequent gratitude themes?**
Yes, the `analyze_theme_distribution` tool identifies which subjects or categories you are most frequently grateful for.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gratitude-journal-analytics](https://vinkius.com/en/ai-agent-connect/gratitude-journal-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gratitude Journal Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gratitude-journal-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gratitude Journal Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gratitude-journal-analytics": {
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
