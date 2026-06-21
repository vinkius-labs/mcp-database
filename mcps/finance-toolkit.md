# Finance Toolkit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/finance-toolkit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Empower your AI agents to compute complex financial formulas. Instantly calculate ROI, compound interests, and SAC/Price amortization tables local.

## Description
Financial mathematics require absolute deterministic precision. A single hallucination by an LLM in an interest rate or loan amortization could lead to disastrous business decisions. The Finance Toolkit MCP Server solves this by delegating the math to an exact V8 Javascript engine.

### The Superpowers
- **Flawless Amortization:** Compare SAC (Constant Amortization) and PRICE (French) loan tables instantly, providing exact summaries without blowing up the context window.
- **Compound Certainty:** Calculate exponential compound interests with customizable frequencies.
- **Investment Tracking:** Reliably compute ROI (Return on Investment) and net profit margins.
- **Absolute Privacy (Local):** Sensitive financial planning data, loan principals, and proprietary rates never leave your local infrastructure.


## Available Tools
- **calculate_amortization**: Rate must be periodic decimal (e.g. monthly rate). Type must be "SAC" or "PRICE".

Generates a summarized amortization schedule (SAC or PRICE table)
- **calculate_compound_interest**: g. 0.05). Frequency is times per year interest is compounded (default 1).

Calculates compound interest over a period of time
- **calculate_roi**: Calculates the Return on Investment (ROI) percentage
- **calculate_simple_interest**: Rate must be decimal (e.g. 0.05 for 5%).

Calculates simple interest over a period of time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Finance Toolkit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to finance a $500,000 property over 360 months at a 0.8% monthly interest rate. Give me the summary using the SAC table."

**🤖 AI Agent:**
> Using the calculate_amortization tool: The first installment is $5,388.89, the last is $1,400.00. Total interest paid will be $722,000.00.

---

**👤 You:**
> "If I invest $10,000 for 5 years with an annual compound interest rate of 7%, what will be the final amount?"

**🤖 AI Agent:**
> Using the calculate_compound_interest tool: The final amount will be $14,025.52, generating $4,025.52 in pure interest.

---

**👤 You:**
> "Calculate the ROI for a marketing campaign where we invested $2,500 and generated $8,700 in sales."

**🤖 AI Agent:**
> Using the calculate_roi tool: The net profit is $6,200, resulting in a phenomenal ROI of 248%.


## ❓ FAQ

**Q: Why doesn't the amortization tool return the full 360-month table?**
Returning 360 lines of JSON would severely bloat the LLM's context window, increasing API costs and causing distraction. We return a "Smart Summary" (total paid, total interest, first and last installments) which is perfect for AI decision-making.

**Q: Are the compound interest calculations precise enough for banking?**
Yes. The underlying engine relies on JavaScript's high-precision floating-point arithmetic (IEEE 754 standard). Outputs are rounded to 2 decimal places specifically for financial display standards.

**Q: Can it compare SAC vs PRICE automatically?**
An AI agent using this MCP can execute the tool twice in parallel—once for SAC and once for PRICE—and instantly write a comparative analysis report for you based on the exact totals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/finance-toolkit](https://vinkius.com/mcp/finance-toolkit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Finance Toolkit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `finance-toolkit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Finance Toolkit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "finance-toolkit": {
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
