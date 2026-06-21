# Scholarship Eligibility Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/scholarship-eligibility-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate household per capita income and determine eligibility for scholarship programs like ProUni and FIES.

## Description
This MCP server provides tools to calculate household per capita income and check eligibility for various scholarship programs. Use `calculate_per_capita_income` to compute the economic share of a household, `check_program_eligibility` to verify if a student qualifies for specific grants based on income thresholds, and `retrieve_program_requirements` to fetch detailed rules and multipliers for programs like PROUNI or FIES.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scholarship Eligibility Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate per capita income for 5000 gross income and 4 members."

**🤖 AI Agent:**
> The calculated per capita income is 1250.

---

**👤 You:**
> "Am I eligible for PROUNI_FULL with 1000 per capita income?"

**🤖 AI Agent:**
> Yes, you are eligible for PROUNI_FULL with 100% coverage.

---

**👤 You:**
> "What are the rules for STATE_GRANT?"

**🤖 AI Agent:**
> The `retrieve_program_requirements` tool shows that STATE_GRANT allows up to 2x the minimum wage.


## ❓ FAQ

**Q: How do I check if I am eligible for ProUni?**
Use the `check_program_eligibility` tool with the `PROUNI_FULL` or `PROUNI_PARTIAL` program type and your calculated per capita income. Tools available: `your_tool_name`.

**Q: What is per capita income?**
It is the total gross family income divided by the number of people living in your household. You can calculate this using the `calculate_per_capita_income` tool.

**Q: Can I check requirements for FIES?**
Yes, use the `retrieve_program_requirements` tool with the `FIES_STANDARD` program type to see the income thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/scholarship-eligibility-checker](https://vinkius.com/mcp/scholarship-eligibility-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scholarship Eligibility Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scholarship-eligibility-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scholarship Eligibility Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scholarship-eligibility-checker": {
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
