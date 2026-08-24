# Mortgage Amortization Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mortgage-amortization-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Generate precise mortgage amortization schedules and calculate payoff acceleration.

## Description
This MCP server provides deterministic tools for mortgage planning. Use `calculate_loan_summary` to find your periodic payment and total interest, `get_payment_breakdown` to inspect the principal and interest split for any specific payment, and `check_pmi_status` to identify when your balance hits the 78% threshold for PMI removal. It handles monthly and bi-weekly frequencies and calculates the impact of extra principal payments on your payoff date.


## Available Tools (3)
- **calculate_loan_summary**: Calculate standard monthly payment, total interest, and time saved with extra payments
- **check_pmi_status**: Check when the 78% PMI removal threshold will be reached
- **get_payment_breakdown**: Get the exact split of principal and interest for a specific payment number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mortgage Amortization Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my monthly payment and total interest for a $300,000 loan at 5% interest for 30 years?"

**🤖 AI Agent:**
> Your monthly payment is $1,610.46, and the total interest paid over the 30-year term will be $279,767.11.

---

**👤 You:**
> "How much of my 47th payment goes to principal for a $300,000 loan at 5% interest for 30 years?"

**🤖 AI Agent:**
> For payment #47, the interest component is $618.45 and the principal component is $992.01, leaving a remaining balance of $287,345.22.

---

**👤 You:**
> "When will I hit the 78% threshold for PMI on a $300,000 loan at 5% interest for 30 years?"

**🤖 AI Agent:**
> You will reach the 78% PMI removal threshold at payment number 214.


## ❓ FAQ

**Q: How can I see how much interest I will pay in total?**
You can use the `calculate_loan_summary` tool, which returns the `totalInterestPaid` for the entire life of the loan.

**Q: Can I calculate how much faster I will pay off my loan with extra payments?**
Yes, by providing an `extraPrincipalPerPeriod` value to `calculate_loan_summary`, the tool will return the `monthsSaved` resulting from your extra payments.

**Q: How do I know when I can remove my Private Mortgage Insurance (PMI)?**
Use the `check_pmi_status` tool. It calculates the specific payment number when your principal balance reaches the 78% threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mortgage-amortization-engine](https://vinkius.com/ai-agent-connect/mortgage-amortization-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mortgage Amortization Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mortgage-amortization-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mortgage Amortization Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mortgage-amortization-engine": {
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
