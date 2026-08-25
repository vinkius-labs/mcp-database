# Cron Expression Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cron-expression-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validate and calculate next execution times for standard and extended cron expressions.

## Description
The Cron Expression Validator is a high-precision tool designed to ensure scheduling accuracy for automated tasks. It supports both the standard 5-field cron format and the extended 6-field format (including seconds). By using `validate_cron_expression`, you can instantly detect syntax errors or range violations, such as an invalid minute value. For complex scheduling needs, `calculate_next_execution` computes the exact next occurrence of a schedule from any given ISO 8601 timestamp. Additionally, `parse_cron_components` allows for deep inspection of each field's pattern, making it easy to debug complex cron strings containing wildcards, ranges, or steps.


## Available Tools (3)
- **parse_cron_components**: Deconstructs a cron expression into its individual parts to allow for detailed inspection
- **validate_cron_expression**: Checks if a provided string is a syntactically correct cron expression and if all values fall within their permitted numerical ranges
- **calculate_next_execution**: Computes the exact next occurrence of a cron schedule after a specific point in time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cron Expression Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this cron expression valid: '*/5 0 * * *'?"

**🤖 AI Agent:**
> Yes, the expression is valid. It is configured to run every 5 minutes during the midnight hour.

---

**👤 You:**
> "When is the next time '0 12 * * *' will run after 2024-01-01T00:00:00Z?"

**🤖 AI Agent:**
> The next execution is scheduled for 2024-01-01T12:00:00Z.

---

**👤 You:**
> "Check if '61 * * * *' is a valid cron expression."

**🤖 AI Agent:**
> The expression is invalid because the minutes field contains '61', which exceeds the maximum allowed value of 59.


## ❓ FAQ

**Q: Does this support the 6-field cron format?**
Yes, by setting the `isExtended` parameter to true in tools like `validate_cron_expression`, you can validate and calculate schedules that include seconds.

**Q: How can I see the individual parts of my cron expression?**
You can use the `parse_cron_components` tool to deconstruct your expression into its constituent fields, such as minutes, hours, and days.

**Q: What happens if my cron expression is invalid?**
The `validate_cron_expression` tool will return `isValid: false` along with a detailed list of `validationErrors` explaining exactly which field failed and why.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cron-expression-validator](https://vinkius.com/ai-agent-connect/cron-expression-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cron Expression Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cron-expression-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cron Expression Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cron-expression-validator": {
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
