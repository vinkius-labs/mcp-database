# Running Pace Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/running-pace-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Convert running paces, predict race times using Riegel formula, and generate training zones.

## Description
This MCP server provides specialized tools for runners to manage their performance and training. Use `convert_units` to switch between metric and imperial units like min/km and mph. With `predict_race_times`, you can estimate future race performances using the Riegel formula based on your current achievements. The `calculate_training_zones` tool helps you plan intensity levels such as easy, tempo, or interval runs relative to your baseline pace. Finally, use `generate_split_table` to create detailed distance and time checkpoints for any race distance.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Pace Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert 5:00 min/km to mph."

**🤖 AI Agent:**
> 5:00 min/km is approximately 7.48 mph.

---

**👤 You:**
> "Predict my marathon time if I ran a 10k in 50 minutes."

**🤖 AI Agent:**
> Based on a 50-minute 10k, your predicted marathon time is approximately 3:52:00.

---

**👤 You:**
> "What should my easy run pace be if my baseline is 6:00 min/km?"

**🤖 AI Agent:**
> Your target easy run pace is between 6:36 and 7:12 min/km.


## ❓ FAQ

**Q: How can I convert my pace from min/km to mph?**
You can use the `convert_units` tool by providing your current pace in min/km and specifying mph as the target unit. Tools available: `your_tool_name`.

**Q: How does the race time prediction work?**
The `predict_race_times` tool uses the Riegel formula to estimate your performance at different distances based on a known completed race.

**Q: Can I calculate my target interval pace?**
Yes, use the `calculate_training_zones` tool with your baseline pace and select 'interval' as the zone type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/running-pace-converter](https://vinkius.com/mcp/running-pace-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Pace Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-pace-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Pace Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-pace-converter": {
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
