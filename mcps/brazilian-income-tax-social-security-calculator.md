# Brazilian Income Tax & Social Security Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brazilian-income-tax-social-security-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Brazilian IRPF and INSS deductions for 2024/2025.

## Description
This MCP server provides a computational engine to calculate Brazilian Individual Income Tax (IRPF) and Social Security (INSS) liabilities. Using tools like `calculate_inss_deduction`, users can determine mandatory deductions from gross earnings. The `evaluate_irpf_liability` tool compares Simplified vs. Complete deduction methods, helping taxpayers find the most advantageous approach for the 2024/2025 fiscal period. Additionally, `generate_payment_metadata` assists in preparing DARF payment information.


## Available Tools (3)
- **calculate_inss_deduction**: Calculate Social Security (INSS) deduction
- **evaluate_irpf_liability**: Evaluate IRPF taxation method
- **generate_payment_metadata**: Generate DARF payment metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brazilian Income Tax & Social Security Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much is my INSS deduction if I earn 3000 BRL monthly?"

**🤖 AI Agent:**
> The calculated INSS deduction for 3,000.00 BRL is approximately 275.40 BRL.

---

**👤 You:**
> "Which method is better for 4000 taxable income with 1000 in deductions and 1 dependent?"

**🤖 AI Agent:**
> The Simplified method results in a lower tax liability compared to the Complete method for this scenario.

---

**👤 You:**
> "What information do I need for my DARF payment for a 500 BRL tax amount in May 2024?"

**🤖 AI Agent:**
> You will need to pay 500.00 BRL by the specified due date, with the description 'Imposto de Renda - Mensal'.


## ❓ FAQ

**Q: How does the INSS calculation work?**
The `calculate_inss_deduction` tool applies progressive rates to your gross earnings up to the established ceiling.

**Q: Can I compare different tax declaration methods?**
Yes, use `evaluate_irpf_liability` to see if the Simplified or Complete method results in lower tax liability.

**Q: Does it handle 13th salary?**
Yes, both INSS and IRPF calculations can be performed specifically for the 13th salary using the appropriate tool parameters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brazilian-income-tax-social-security-calculator](https://vinkius.com/mcp/brazilian-income-tax-social-security-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brazilian Income Tax & Social Security Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brazilian-income-tax-social-security-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brazilian Income Tax & Social Security Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brazilian-income-tax-social-security-calculator": {
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
