# US Non-Compete Enforceability Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-non-compete-enforceability-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [legal](../categories/legal.md)

Assess the legal enforceability of non-compete agreements across US states.

## Description
This MCP server provides specialized tools to evaluate whether a non-compete clause is enforceable, partially enforceable, or void based on US state laws. Use `check_state_legality` to identify states with total statutory bans like California or Minnesota. Use `evaluate_noncompete_clause` to perform a detailed assessment using duration and geographic radius parameters. You can also use `get_enforceability_guidelines` to retrieve the maximum reasonable thresholds for specific jurisdictions.


## Available Tools
- **check_state_legality**: Checks if a US state has a statutory ban on non-competes
- **evaluate_noncompete_clause**: Evaluates the enforceability of a non-compete clause
- **get_enforceability_guidelines**: Retrieves general non-compete enforceability thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Non-Compete Enforceability Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a non-compete valid in California?"

**🤖 AI Agent:**
> Using `check_state_legality` for California returns a status of 'Prohibited' because it is under a total statutory ban.

---

**👤 You:**
> "Evaluate a 18-month non-compete with a 75-mile radius in Texas."

**🤖 AI Agent:**
> The `evaluate_noncompete_clause` tool would classify this as 'partially_enforceable' because the duration and radius fall within moderate threshold ranges.

---

**👤 You:**
> "What are the guidelines for non-competes in Florida?"

**🤖 AI Agent:**
> By calling `get_enforceability_guidelines` for Florida, you can retrieve the specific maximum reasonable duration and radius allowed before a clause is considered risky.


## ❓ FAQ

**Q: What does it mean if a state is 'banned'?**
A banned status means the state has passed legislation that prohibits all non-compete agreements, making them legally void regardless of other terms.

**Q: How is enforceability determined?**
Enforceability is assessed by checking the state's legality, the duration of the restriction in months, and the geographic radius in miles against established reasonableness standards.

**Q: Can I check specific thresholds for my state?**
Yes, use the `get_enforceability_guidelines` tool to find the maximum reasonable duration and radius for a specific US state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-non-compete-enforceability-analyzer](https://vinkius.com/mcp/us-non-compete-enforceability-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Non-Compete Enforceability Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-non-compete-enforceability-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Non-Compete Enforceability Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-non-compete-enforceability-analyzer": {
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
