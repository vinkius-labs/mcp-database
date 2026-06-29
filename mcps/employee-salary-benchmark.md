# Employee Salary Benchmark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/employee-salary-benchmark)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Retrieve market salary ranges in USD and BRL for various roles, seniority levels, and startup stages.

## Description
The Employee Salary Benchmark MCP connects AI agents to a specialized dataset of market compensation. By using tools like `get_salary_range`, `compare_seniority_premium`, and `calculate_average_salary`, you can access precise salary bounds (min/max) in both USD and BRL. This tool is essential for analyzing compensation trends across different professional roles, seniority levels, geographic hubs like San Francisco or London, and startup funding stages from pre-seed to Series B.


## Available Tools (3)
- **calculate_average_salary**: Calculate the average minimum salary for a list of roles
- **get_salary_range**: Retrieve the minimum and maximum salary bounds for a professional profile
- **compare_seniority_premium**: Calculate the estimated salary increase when moving between seniority levels


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Employee Salary Benchmark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the salary range for a mid-level designer in London at a seed stage startup?"

**🤖 AI Agent:**
> For a mid-level designer in London at the seed stage, the estimated salary range is $60,000 - $85,000 USD ($300,000 - $425,000 BRL).

---

**👤 You:**
> "How much more can I expect to earn if I move from a junior to a senior engineer role in San Francisco?"

**🤖 AI Agent:**
> Moving from junior to senior level in San Francisco typically results in an estimated 45% increase in the middle of the salary range.

---

**👤 You:**
> "Compare the average salaries for engineers and designers in Berlin at Series A stage."

**🤖 AI Agent:**
> The average salary for engineers is $75,000 USD, while for designers it is $65,000 USD at the Series A stage in Berlin.


## ❓ FAQ

**Q: How can I find the salary range for a Software Engineer in San Francisco?**
Use the `get_salary_range` tool with the parameters: role='engineer', seniority='mid', city='sanFrancisco', and stage='seed'.

**Q: Can I compare salary increases between different seniority levels?**
Yes, the `compare_seniority_premium` tool calculates the estimated percentage increase and range expansion when moving from one level to another.

**Q: Does the tool provide salaries in Brazilian Real (BRL)?**
Yes, all salary bounds returned by `get_salary_range` include both USD and BRL values based on a fixed internal exchange rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/employee-salary-benchmark](https://vinkius.com/mcp/employee-salary-benchmark)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Employee Salary Benchmark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `employee-salary-benchmark` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Employee Salary Benchmark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "employee-salary-benchmark": {
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
