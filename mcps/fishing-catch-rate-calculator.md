# Fishing Catch Rate Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fishing-catch-rate-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate fishing productivity and catch rates per hour.

## Description
This MCP server provides tools to analyze fishing efficiency. Use `get_catch_rate` to find the catch per hour for a single session, `get_session_summary` to aggregate multiple records, `validate_fishing_efficiency` to check if you've met your goals, and `compare_locations` to see which spot is more productive.


## Available Tools (4)
- **compare_locations**: Compares the productivity of two different fishing locations or methods
- **get_catch_rate**: Calculates the catch rate for a specific fishing session
- **get_session_summary**: Provides a high-level overview of fishing productivity
- **validate_fishing_efficiency**: Checks if a specific catch rate meets a target efficiency goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fishing Catch Rate Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I caught 15 fish in 3 hours. What is my catch rate?"

**🤖 AI Agent:**
> Your catch rate is 5.0 fish per hour.

---

**👤 You:**
> "My current catch rate is 4.5 per hour. Is this enough to meet my target of 5.0?"

**🤖 AI Agent:**
> No, you have not met the target. The efficiency gap is 0.5.

---

**👤 You:**
> "Which location is better: Location A with 10 fish in 2 hours, or Location B with 12 fish in 4 hours?"

**🤖 AI Agent:**
> Location A is more productive with a rate of 5.0 fish per hour compared to Location B's 3.0 fish per hour.


## ❓ FAQ

**Q: How do I calculate my catch per hour?**
You can use the `get_catch_rate` tool by providing the total number of fish caught and the total hours spent fishing.

**Q: Can I compare two different fishing spots?**
Yes, use the `compare_locations` tool to determine which location has higher productivity.

**Q: How can I see my overall performance across many trips?**
The `get_session_summary` tool allows you to aggregate multiple catch records into a single overview.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fishing-catch-rate-calculator](https://vinkius.com/en/ai-agent-connect/fishing-catch-rate-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fishing Catch Rate Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fishing-catch-rate-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fishing Catch Rate Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fishing-catch-rate-calculator": {
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
