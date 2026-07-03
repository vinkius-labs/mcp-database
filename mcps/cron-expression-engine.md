# Cron Expression Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cron-expression-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Parse, validate, convert, and generate cron expressions across multiple standards.

## Description
The Cron Expression Engine is a powerful utility for managing complex scheduling patterns. It acts as a bridge between natural language and formal cron syntax, supporting multiple standards including Unix, Quartz (Spring), AWS CloudWatch, and GitHub Actions. Use `parse_and_explain` to break down any expression into human-readable parts, `validate_cron` to ensure your syntax is correct for its specific format, `convert_format` to transform expressions between different standards without losing temporal meaning, and `calculate_schedule` to predict future or past execution timestamps. This tool is essential for developers managing automated tasks, CI/CD pipelines, or cloud-native event rules.


## Available Tools (4)
- **calculate_schedule**: Calculate upcoming or recent timestamps based on a cron expression
- **convert_format**: Convert a cron expression from one format to another
- **parse_and_explain**: Parse a cron expression and get field explanations
- **validate_cron**: Validate the syntax of a cron expression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cron Expression Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Explain this cron expression: '0 9 * * 1-5' in unix format."

**🤖 AI Agent:**
> The schedule '0 9 * * 1-5' means: At 09:00 AM, Monday through Friday.

---

**👤 You:**
> "Is '65 * * * *' a valid unix cron expression?"

**🤖 AI Agent:**
> No, the value 65 is out of range for minutes (must be between 0 and 59).

---

**👤 You:**
> "Convert '0 12 * * *' from unix to quartz format."

**🤖 AI Agent:**
> The converted Quartz expression is '0 0 12 * * ?'.


## ❓ FAQ

**Q: What cron formats are supported?**
The engine supports Unix (5-field), Quartz (6 or 7-field), AWS CloudWatch, and GitHub Actions formats.

**Q: How can I check if my cron expression is valid?**
You can use the `validate_cron` tool. Simply provide your expression and specify which format (e.g., 'unix' or 'aws') you are using.

**Q: Can I convert a Unix cron to AWS CloudWatch format?**
Yes, the `convert_format` tool is designed specifically for this. It handles the structural differences between standards while maintaining the same schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cron-expression-engine](https://vinkius.com/mcp/cron-expression-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cron Expression Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cron-expression-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cron Expression Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cron-expression-engine": {
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
