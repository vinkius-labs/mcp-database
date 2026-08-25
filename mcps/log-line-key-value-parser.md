# Log Line Key-Value Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/log-line-key-value-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Extracts structured data and character offsets from unstructured log lines.

## Description
This MCP server provides precise tools for transforming unstructured log text into structured data. It identifies log families like Syslog or Apache/Nginx access logs and extracts exact key-value pairs. By using `parse_log_line`, you can retrieve structured fields along with their exact character offsets. You can also use `identify_format` to quickly detect log types or `get_field_metadata` to inspect specific field details like value and type.


## Available Tools (3)
- **get_field_metadata**: 
- **parse_log_line**: 
- **identify_format**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Log Line Key-Value Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Parse this log line: 'Oct 11 22:14:15 host1 syslogd: user login success'"

**🤖 AI Agent:**
> { "format": "syslog", "fields": { "timestamp": { "value": "Oct 11 22:14:15", "start": 0, "end": 15 }, "hostname": { "value": "host1", "start": 16, "end": 20 }, "process": { "value": "syslogd", "start": 21, "end": 27 }, "message": { "value": "user login success", "start": 29, "end": 46 } } }

---

**👤 You:**
> "What type of log is this: '127.0.0.1 - - [10/Oct/2000:13:55:36 -0700] "GET /index.html HTTP/1.0" 200 2326'"

**🤖 AI Agent:**
> { "format": "apache_access", "confidence": 0.98 }

---

**👤 You:**
> "Extract the status code from this parsed data: {"format": "nginx_access", "fields": {"status": {"value": "404", "start": 50, "end": 53}}}"

**🤖 AI Agent:**
> { "value": "404", "start": 50, "end": 53, "type": "number" }


## ❓ FAQ

**Q: What log formats are supported?**
The server supports Syslog, Apache access logs, Nginx access logs, and generic key-value patterns.

**Q: How do I get the position of a specific field?**
Use the `get_field_metadata` tool after running `parse_log_line` to retrieve the exact start and end character offsets.

**Q: Can it handle unknown log formats?**
Yes, if a format is not recognized, the tool attempts to extract generic key-value pairs from the string.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/log-line-key-value-parser](https://vinkius.com/ai-agent-connect/log-line-key-value-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Log Line Key-Value Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `log-line-key-value-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Log Line Key-Value Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "log-line-key-value-parser": {
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
