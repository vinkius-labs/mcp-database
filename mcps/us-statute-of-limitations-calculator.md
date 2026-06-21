# US Statute of Limitations Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-statute-of-limitations-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Calculate US legal filing deadlines based on claim type, state, and accrual date.

## Description
This MCP server provides precise tools for determining the statute of limitations for various legal actions across US states. Use `calculate_statute_deadline` to find standard deadlines for contract, tort, or fraud claims. The server also supports evaluating the discovery rule via `evaluate_discovery_rule` and assessing how tolling events like minority or incapacity might extend your deadline using `check_tolling_impact`.


## Available Tools
- **check_tolling_impact**: Identifies if any known tolling events have extended the existing deadline
- **calculate_statute_deadline**: Determines the standard filing deadline based on claim type, state, and the date of the incident
- **evaluate_discovery_rule**: Re-calculates a deadline based on the moment the harm was discovered


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Statute of Limitations Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the statute of limitations for a breach of contract in California that occurred on 2023-01-01."

**🤖 AI Agent:**
> The calculated deadline for your contract claim in CA is 2026-01-01.

---

**👤 You:**
> "What happens if I discovered a fraud on 2024-05-20 that originally occurred on 2020-01-01 in New York?"

**🤖 AI Agent:**
> The revised deadline based on the discovery rule is 2030-05-20.

---

**👤 You:**
> "Check if a tolling event on 2022-06-15 extends my current deadline of 2024-01-01."

**🤖 AI Agent:**
> The extended deadline after accounting for the tolling event is 2025-06-15.


## ❓ FAQ

**Q: What claim types are supported?**
The calculator supports contract, tort, and fraud claims.

**Q: How does the discovery rule work in this tool?**
The `evaluate_discovery_rule` tool allows you to recalculate a deadline based on when the harm was discovered rather than when it occurred.

**Q: Can I check for tolling extensions?**
Yes, use the `check_tolling_impact` tool to see if events like reaching the age of majority or mental incapacity extend your filing deadline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-statute-of-limitations-calculator](https://vinkius.com/mcp/us-statute-of-limitations-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Statute of Limitations Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-statute-of-limitations-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Statute of Limitations Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-statute-of-limitations-calculator": {
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
