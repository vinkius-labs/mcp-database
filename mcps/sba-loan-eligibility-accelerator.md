# SBA Loan Eligibility Accelerator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sba-loan-eligibility-accelerator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze SBA loan eligibility and portfolio potential for small businesses.

## Description
This MCP server provides tools to evaluate Small Business Administration (SBA) loan eligibility. It allows users to check if specific industries are permitted, evaluate individual company profiles against size and revenue standards, and aggregate data to assess the total loan potential across an entire portfolio. Use `check_industry_eligibility` to verify sector permissions, `evaluate_company_eligibility` for detailed company assessments, and `analyze_portfolio_potential` to summarize opportunities across multiple companies.


## Available Tools (3)
- **analyze_portfolio_potential**: Analyze portfolio potential
- **check_industry_eligibility**: Check if industry is SBA eligible
- **evaluate_company_eligibility**: Evaluate company for SBA loan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SBA Loan Eligibility Accelerator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the manufacturing industry eligible for SBA loans?"

**🤖 AI Agent:**
> Yes, manufacturing is a permitted industry for SBA financing.

---

**👤 You:**
> "A company has $500,000 revenue, 10 employees, is in Retail, and needs $50,000 for Working Capital. Are they eligible?"

**🤖 AI Agent:**
> Yes, the company is eligible for an SBA loan with a maximum potential amount of $50,000.

---

**👤 You:**
> "What is the total potential loan amount for a portfolio of 3 eligible companies with max amounts of $100k, $200k, and $150k?"

**🤖 AI Agent:**
> The total potential loan amount for the portfolio is $450,000.


## ❓ FAQ

**Q: How do I check if my industry is eligible for an SBA loan?**
You can use the `check_industry_eligibility` tool to determine if your specific industry is permitted under SBA guidelines.

**Q: Can I analyze multiple companies at once?**
Yes, the `analyze_portfolio_potential` tool is designed to aggregate data and provide a summary of eligibility and loan amounts for a group of companies.

**Q: What factors determine a company's eligibility?**
Eligibility is determined by industry classification, annual revenue, employee count, and the intended purpose of the loan via the `evaluate_company_eligibility` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sba-loan-eligibility-accelerator](https://vinkius.com/ai-agent-connect/sba-loan-eligibility-accelerator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SBA Loan Eligibility Accelerator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sba-loan-eligibility-accelerator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SBA Loan Eligibility Accelerator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sba-loan-eligibility-accelerator": {
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
