# Words Per Minute Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/words-per-minute-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate typing and reading speed with precision.

## Description
This MCP server provides precise tools for calculating words per minute (WPM) for both typing and reading tasks. It includes tools to `calculate_wpm` for individual attempts, `get_speed_category` to determine qualitative speed tiers, `validate_input_metrics` to ensure data is physically possible, and `batch_calculate_wpm` to analyze multiple performance attempts at once.


## Available Tools (4)
- **batch_calculate_wpm**: Pass attempts as a JSON string array of objects with wordCount and durationInSeconds.

Processes a list of multiple speed attempts to provide an overview of performance
- **calculate_wpm**: Calculates the typing or reading speed based on the amount of text processed and the time taken
- **get_speed_category**: Determines the qualitative speed tier for a given WPM value
- **validate_input_metrics**: Ensures that the provided word counts and time metrics are logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Words Per Minute Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I typed 300 words in 60 seconds. What is my WPM and category?"

**🤖 AI Agent:**
> Your speed is 300 WPM, which falls into the Elite category.

---

**👤 You:**
> "Calculate my average speed for these attempts: 100 words in 120s, and 150 words in 60s."

**🤖 AI Agent:**
> Your average speed is 125 WPM.

---

**👤 You:**
> "Is it possible to type 5000 words in 10 seconds?"

**🤖 AI Agent:**
> No, that speed is not physically possible for a human.


## ❓ FAQ

**Q: How is WPM calculated?**
The `calculate_wpm` tool calculates speed by dividing the total word count by the duration in minutes.

**Q: Can I analyze multiple typing tests at once?**
Yes, you can use `batch_calculate_wpm` to get aggregate statistics like average, max, and min speed from a list of attempts.

**Q: How are speed categories determined?**
The `get_speed_category` tool assigns a tier such as Slow, Average, Fast, or Elite based on industry standard thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/words-per-minute-calculator](https://vinkius.com/en/ai-agent-connect/words-per-minute-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Words Per Minute Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `words-per-minute-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Words Per Minute Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "words-per-minute-calculator": {
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
