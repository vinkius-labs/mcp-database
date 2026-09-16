# Surf Performance Journaling System MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-performance-journaling-system)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A structured system to design surf performance journals, balancing qualitative feel with quantitative metrics.

## Description
This MCP server provides a complete toolkit for surfers to design personalized performance journals. It uses a specialized design methodology to synthesize tracking goals, session frequency, and specific metrics into a cohesive workflow. Users can use `generate_journal_template` to create a full system including entry structures and review schedules. The toolkit also includes `analyze_entry_composition` to ensure a healthy balance between subjective 'feel' and objective data, `calculate_review_cadence` to optimize review timing, and `validate_metric_relevance` to ensure all tracked data points directly support the surfer's primary objectives.


## Available Tools (4)
- **analyze_entry_composition**: Evaluates if a proposed journal entry structure provides enough balance between qualitative and quantitative data
- **calculate_review_cadence**: Determines the optimal timing for performance reviews to prevent data overload or loss of momentum
- **generate_journal_template**: Creates a complete performance journaling system based on user preferences
- **validate_metric_relevance**: Checks if the selected metrics actually support the stated tracking goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Performance Journaling System** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I surf twice a week and want to improve my wave reading and paddle endurance. I want to track wave count and session duration. Can you build me a journal?"

**🤖 AI Agent:**
> I have generated your Surf Performance Journal. It includes a weekly review schedule and an entry structure that captures your wave count, session duration, and qualitative notes on wave reading feel.

---

**👤 You:**
> "Is my journal entry structure balanced? I am tracking wave count, turn count, and session duration."

**🤖 AI Agent:**
> Your current structure is heavily quantitative. To achieve a balanced journal, you should add at least one qualitative field, such as 'Water Conditions' or 'Board Feel', to complement your three quantitative metrics.

---

**👤 You:**
> "I surf daily. How often should I review my data if I am tracking many different metrics?"

**🤖 AI Agent:**
> Since you surf daily with high tracking complexity, a daily or bi-weekly short review is recommended to maintain relevance and prevent data overload.


## ❓ FAQ

**Q: How do I create my first journal template?**
You can use the `generate_journal_template` tool by providing your tracking goals, how often you surf, and the metrics you want to capture.

**Q: How often should I review my performance data?**
The optimal review timing is determined by the `calculate_review_cadence` tool, which considers your surfing frequency and the complexity of your metrics.

**Q: Can I check if my metrics are actually useful for my goals?**
Yes, the `validate_metric_relevance` tool evaluates if your selected metrics provide a measurable or descriptive way to track progress toward your specific goals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-performance-journaling-system](https://vinkius.com/en/ai-agent-connect/surf-performance-journaling-system)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Performance Journaling System** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-performance-journaling-system` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Performance Journaling System** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-performance-journaling-system": {
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
