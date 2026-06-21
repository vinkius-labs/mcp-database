# StatHat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stathat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Track custom metrics and statistics effortlessly via StatHat — post counters, values, and batch updates directly from your AI agent.

## Description
Connect your **StatHat** account to any AI agent to monitor your application's performance and business metrics through simple commands.

### What you can do

- **EZ Statistics** — Post stats using just a name (e.g., "User Signups"). StatHat automatically creates the metric if it doesn't exist.
- **Classic Counters** — Increment specific metrics using unique Stat Keys for precise tracking.
- **Value Tracking** — Send numerical values (like response times or temperatures) to specific stat keys.
- **Batch Processing** — Use the JSON API to send multiple statistics in a single request for high-efficiency logging.

### How it works

1. Subscribe to this server
2. Enter your StatHat EZ Key or User Key
3. Start logging metrics from Claude, Cursor, or any MCP-compatible client

No more manual dashboard entries or complex SDK configurations for quick tracking. Your AI acts as a bridge to your data observability stack.

### Who is this for?

- **Developers** — log errors, function execution counts, or performance metrics directly from the IDE.
- **Data Analysts** — quickly update business KPIs or experimental results via natural language.
- **DevOps Engineers** — monitor system health and event counts without leaving the terminal or chat interface.


## Available Tools
- **post_classic_counter**: Post a counter stat using the StatHat Classic API
- **post_classic_value**: Post a value stat using the StatHat Classic API
- **post_ez_stat**: Creates the stat automatically if it does not exist.

Post a stat using the StatHat EZ API
- **post_json_stats**: Pass a JSON array of objects containing stat/key, count/value, and optional t (timestamp).

Post multiple stats using the StatHat JSON API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **StatHat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Increment the 'Messages Processed' stat by 1 using StatHat EZ."

**🤖 AI Agent:**
> I've successfully incremented the 'Messages Processed' counter. StatHat confirmed the update was received.

---

**👤 You:**
> "Post a value of 45.5 to the stat key 'th789abc' using the classic API."

**🤖 AI Agent:**
> The value 45.5 has been posted to stat key 'th789abc'. Your dashboard should reflect this update immediately.

---

**👤 You:**
> "Batch update these stats: 'errors' count 5 and 'latency' value 120."

**🤖 AI Agent:**
> I've sent the batch update for 'errors' and 'latency' via the JSON API. Both metrics have been updated.


## ❓ FAQ

**Q: What is the difference between the EZ API and the Classic API?**
The EZ API (`post_ez_stat`) allows you to post stats using a simple human-readable name and your EZ Key. The Classic API (`post_classic_counter`, `post_classic_value`) requires a unique Stat Key for each specific metric, providing more granular control.

**Q: Do I need to create a stat on the website before posting to it?**
No! When using the `post_ez_stat` tool, StatHat will automatically create the statistic for you if it doesn't already exist in your account.

**Q: Can I send multiple metrics at once to save time?**
Yes, you can use the `post_json_stats` tool to send an array of multiple stat updates in a single network request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stathat](https://vinkius.com/mcp/stathat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **StatHat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stathat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **StatHat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stathat": {
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
