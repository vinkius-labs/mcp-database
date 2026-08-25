# Accelerator Venture Debt Readiness MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-venture-debt-readiness)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Assess portfolio companies for venture debt eligibility and capacity.

## Description
This MCP server provides tools for accelerators to evaluate the venture debt readiness of their portfolio companies. It calculates debt capacity, assesses individual company eligibility based on revenue and term constraints, and simulates the impact of proposed debt packages on warrant dilution and covenant headroom. Use `calculate_portfolio_readiness` for an aggregate view, `assess_company_readiness` for specific company analysis, or `simulate_debt_impact` to model financial outcomes.


## Available Tools (3)
- **assess_company_readiness**: Evaluates a single company to determine if it is eligible for venture debt and calculates its specific capacity
- **calculate_portfolio_readiness**: Provides a high-level summary of the entire portfolio's readiness for debt deployment
- **simulate_debt_impact**: Predicts how a specific debt package will affect a company's financial position


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Venture Debt Readiness** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total debt capacity for my portfolio?"

**🤖 AI Agent:**
> The total debt capacity for your portfolio is $15,000,000 across 8 debt-ready companies.

---

**👤 You:**
> "Is Company A ready for a $2M debt facility?"

**🤖 AI Agent:**
> Company A is debt-ready with a calculated capacity of $2,500,000, meeting all current term constraints.

---

**👤 You:**
> "How will a $5M loan with 2% warrants affect my company's cash headroom?"

**🤖 AI Agent:**
> The proposed $5,000,000 debt will result in 2% warrant dilution and leave a covenant headroom of $450,000.


## ❓ FAQ

**Q: How do I check the total readiness of my portfolio?**
You can use the `calculate_portfolio_readiness` tool to get a summary including total debt capacity and the count of debt-ready companies.

**Q: Can I simulate how much equity a debt deal will cost?**
Yes, the `simulate_debt_impact` tool predicts projected warrant dilution and evaluates covenant headroom for a proposed debt amount.

**Q: What determines if a company is considered 'debt-ready'?**
A company is debt-ready if it has positive calculated capacity and satisfies all provided term constraints, such as minimum cash covenants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-venture-debt-readiness](https://vinkius.com/ai-agent-connect/accelerator-venture-debt-readiness)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Venture Debt Readiness** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-venture-debt-readiness` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Venture Debt Readiness** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-venture-debt-readiness": {
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
