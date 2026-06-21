# Contract Notice Period Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contract-notice-period-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Calculate minimum legal notice periods and effective termination dates for various contract types across USA and Europe.

## Description
This MCP server provides a precise engine to determine the mandatory minimum notice periods and calculate exact termination dates. By using tools like `get_notice_requirement`, you can retrieve legal requirements for employment, commercial leases, and service agreements across specific US states and European nations. Additionally, use `calculate_effective_date` to find the final day of a contract based on your notice date, or `check_jurisdiction_validity` to verify if a region is within the supported regulatory scope.


## Available Tools (3)
- **get_notice_requirement**: Retrieves the mandatory minimum notice period and its associated legal description
- **calculate_effective_date**: Determines the exact date a contract will end
- **check_jurisdiction_validity**: Validates if a provided location is within the supported legal scope


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contract Notice Period Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum notice period for an employment contract in California?"

**🤖 AI Agent:**
> The `get_notice_requirement` tool would be used to retrieve the specific days and legal description for California.

---

**👤 You:**
> "Calculate the end date if I gave notice on 2024-01-01 with a 30 day period."

**🤖 AI Agent:**
> The `calculate_effective_date` tool will return the calculated termination date based on those inputs.

---

**👤 You:**
> "Is Germany a supported jurisdiction?"

**🤖 AI Agent:**
> You can use `check_jurisdiction_validity` to confirm if Germany is within the supported scope and see its regulatory level.


## ❓ FAQ

**Q: What contract types are supported?**
The server supports employment, commercial lease, and service agreement contracts.

**Q: Which jurisdictions are covered?**
The engine covers various states in the USA and national-level regulations across Europe.

**Q: How do I calculate a termination date?**
Use the `calculate_effective_date` tool by providing the notice date in YYYY-MM-DD format and the number of days in the notice period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contract-notice-period-calculator](https://vinkius.com/mcp/contract-notice-period-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contract Notice Period Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contract-notice-period-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contract Notice Period Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contract-notice-period-calculator": {
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
