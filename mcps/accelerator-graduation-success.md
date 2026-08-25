# Accelerator Graduation Success MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-graduation-success)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates cohort performance metrics including funding success, average raises, and survival rates.

## Description
This MCP server provides a suite of analytical tools for venture accelerator managers to evaluate cohort performance. It calculates critical success indicators such as funding success rates and average capital raised using `calculate_funding_metrics`. It also tracks company outcomes through `calculate_exit_and_survival_metrics` to determine survival, acquisition, and shutdown rates. Additionally, users can scale funding data with `apply_follow_on_adjustment` to account for subsequent funding momentum.


## Available Tools (3)
- **calculate_funding_metrics**: Answers how effectively the cohort is attracting capital and the average scale of those investments
- **apply_follow_on_adjustment**: Adjusts raw funding metrics to account for the momentum of subsequent funding rounds
- **calculate_exit_and_survival_metrics**: Answers how many companies are still operating versus those that have exited or failed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Graduation Success** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the funding metrics for a cohort of 50 companies where 20 raised a total of $10,000,000."

**🤖 AI Agent:**
> The funding success rate is 40% and the average raise is $500,000.

---

**👤 You:**
> "In a cohort of 30 companies, 5 were acquired and 2 shut down. What are the survival, acquisition, and shutdown rates?"

**🤖 AI Agent:**
> The survival rate is 76.67%, the acquisition rate is 16.67%, and the shutdown rate is 6.67%.

---

**👤 You:**
> "Adjust an average raise of $200,000 with a follow-on multiplier of 1.5."

**🤖 AI Agent:**
> The adjusted average raise is $300,000.


## ❓ FAQ

**Q: How is the funding success rate calculated?**
The funding success rate is the number of companies that successfully raised funds divided by the total cohort size, as determined by `calculate_funding_metrics`.

**Q: What is the difference between survival and acquisition rates?**
Survival rate represents companies that are still active and independent, while acquisition rate tracks companies bought by other entities. Both are calculated via `calculate_exit_and_survival_metrics`.

**Q: Can I adjust the average raise for follow-on funding?**
Yes, you can use `apply_follow_on_adjustment` to scale the base average raise by a multiplier representing follow-on performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-graduation-success](https://vinkius.com/ai-agent-connect/accelerator-graduation-success)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Graduation Success** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-graduation-success` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Graduation Success** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-graduation-success": {
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
