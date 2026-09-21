# Audiobook Duration Aggregator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/audiobook-duration-aggregator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total, average, and statistical audiobook listening times.

## Description
This MCP server provides tools to manage and analyze audiobook listening durations. Use `get_total_listening_time` to sum multiple book lengths, `get_average_book_length` to find the mean duration, `get_duration_statistics` to identify the longest and shortest books, and `validate_duration_format` to ensure time strings follow the HH:MM:SS standard.


## Available Tools (4)
- **get_total_listening_time**: Calculates the combined duration of a list of provided audiobooks
- **validate_duration_format**: Checks if a specific time string adheres to the required standard
- **get_average_book_length**: Determines the mean listening time across a collection of audiobooks
- **get_duration_statistics**: Provides a high-level overview of a collection, including the longest and shortest books


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Audiobook Duration Aggregator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total listening time for books lasting 01:00:00, 02:30:00, and 00:45:00?"

**🤖 AI Agent:**
> The total listening time is 04:15:00.

---

**👤 You:**
> "What is the average length of these audiobooks: 01:00:00, 02:00:00, and 03:00:00?"

**🤖 AI Agent:**
> The average length is 02:00:00.

---

**👤 You:**
> "Give me the statistics for books with durations 00:30:00, 05:00:00, and 01:15:00."

**🤖 AI Agent:**
> The longest book is 05:00:00, the shortest is 00:30:00, and the duration range is 4500 seconds.


## ❓ FAQ

**Q: What time format should I use?**
All durations must be provided in the HH:MM:SS format (e.g., 01:30:00 for one hour and thirty minutes).

**Q: How can I check if my duration string is valid?**
You can use the `validate_duration_format` tool to verify if a specific time string adheres to the required standard.

**Q: Can I get the total time for a large collection of books?**
Yes, the `get_total_listening_time` tool is designed to aggregate the total duration of any number of provided audiobook strings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/audiobook-duration-aggregator](https://vinkius.com/en/ai-agent-connect/audiobook-duration-aggregator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Audiobook Duration Aggregator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `audiobook-duration-aggregator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Audiobook Duration Aggregator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "audiobook-duration-aggregator": {
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
