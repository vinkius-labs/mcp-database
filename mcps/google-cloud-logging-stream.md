# Google Cloud Logging Stream MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-logging-stream)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it queries logs using Google Cloud Logging. That's its only function, and nothing else. Incredible for giving your AI secure observability.

## Description
This server strips away dangerous global GCP permissions. It gives your AI agent one surgical superpower: **the ability to run scoped queries on Google Cloud Logging for specific resources.**

By strictly scoping access, your AI can safely troubleshoot application errors, analyze traffic spikes, and monitor infrastructure without ever gaining access to sensitive audit trails globally.

### The Superpowers

- **Absolute Containment:** The agent is strictly limited to query specific logs using your precise filter setup.
- **Native Logging Querying:** Supports full Cloud Logging syntax, allowing the AI to filter, parse JSON payloads, and extract insights.
- **Plug & Play Troubleshooting:** Instantly gives your agent the eyes and ears it needs to debug production issues autonomously.


## Available Tools
- **stream_logs**: You can optionally filter them using advanced GCP Logging filter syntax (e.g., severity>=ERROR).

Read and search log entries from the configured Google Cloud Log


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Cloud Logging Stream** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the last 100 log entries from our configured log stream."

**🤖 AI Agent:**
> I've retrieved the latest 100 entries. They are mostly standard info-level logs, but I noticed a warning around 10:14 AM.

---

**👤 You:**
> "Stream logs filtering only for 'severity>=ERROR'."

**🤖 AI Agent:**
> I found 3 matching error logs. The most recent one indicates a database connection timeout.

---

**👤 You:**
> "Search the logs for the user ID 'user_8819' in the JSON payload."

**🤖 AI Agent:**
> Applying the filter `jsonPayload.userId="user_8819"`, I found the specific event where the user triggered the payment webhook.


## ❓ FAQ

**Q: Why limit the agent to a single Log Name?**
To enforce zero-trust security. An autonomous AI agent debugging an application shouldn't have access to read your organization's entire audit log history, IAM logs, or logs from other unrelated services.

**Q: Can I use advanced GCP Log queries?**
Yes! You can pass any standard GCP Logging filter (e.g., `textPayload:"Exception"` or `jsonPayload.status="500"`) via the `filter` argument. The server automatically merges your filter with the strict `logName` restriction.

**Q: How are the results ordered?**
Results are always returned in descending order (`timestamp desc`), meaning the AI agent gets the most recent logs first, which is ideal for real-time debugging.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-logging-stream](https://vinkius.com/mcp/google-cloud-logging-stream)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Cloud Logging Stream** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-cloud-logging-stream` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Cloud Logging Stream** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-cloud-logging-stream": {
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
