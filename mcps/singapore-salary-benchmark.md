# Singapore Salary Benchmark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/singapore-salary-benchmark)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate your salary percentile rank against Singapore market benchmarks.

## Description
This MCP server provides deterministic salary benchmarking for the Singapore market. It uses Ministry of Manpower (MOM) age-banded medians and industry-specific multipliers to calculate your exact percentile rank and career trajectory score. Use `calculate_salary_percentile` to get a full report including your industry-adjusted median and trajectory status.


## Available Tools (3)
- **get_age_band_median**: Retrieves the base Singapore Ministry of Manpower (MOM) median salary for a specific age group
- **calculate_salary_percentile**: Determines a user's salary percentile rank, industry-adjusted median, and career trajectory score
- **get_industry_multiplier**: Retrieves the specific economic multiplier associated with a given industry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Singapore Salary Benchmark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my salary percentile if I am 28 years old, have 5 years of experience, earn 6000 SGD, and work in tech?"

**🤖 AI Agent:**
> Your percentile rank is 82%, your industry-adjusted median is 5850 SGD, and your career trajectory is On Track.

---

**👤 You:**
> "Calculate my benchmark for a 24-year-old in F&B earning 3000 SGD."

**🤖 AI Agent:**
> Your percentile rank is 47%, your industry-adjusted median is 2800 SGD, and your career trajectory is Below Benchmark.

---

**👤 You:**
> "Check the industry multiplier for the finance sector."

**🤖 AI Agent:**
> The multiplier for the finance industry is 1.4.


## ❓ FAQ

**Q: How is the salary percentile calculated?**
The percentile is calculated by comparing your monthly salary to an industry-adjusted median, which is derived from MOM age-banded data and sector-specific multipliers.

**Q: What industries are supported?**
Supported industries include tech, finance, healthcare, education, f_and_b, and retail.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/singapore-salary-benchmark](https://vinkius.com/ai-agent-connect/singapore-salary-benchmark)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Singapore Salary Benchmark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `singapore-salary-benchmark` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Singapore Salary Benchmark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "singapore-salary-benchmark": {
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
