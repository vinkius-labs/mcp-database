# ECB Interest Rates — Monetary Policy Rates & Banking MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecb-interest-rates-monetary-policy-rates-banking)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

ECB key policy rates: the Main Refinancing Operations rate (MRO), Deposit Facility Rate (DFR), Marginal Lending Facility, all three rates combined, and MFI bank lending/deposit rates showing monetary policy transmission across the eurozone.

## Description
ECB monetary policy rates.

### 5 Tools
- **MRO** — Main Refinancing Operations rate
- **DFR** — Deposit Facility Rate
- **MLFR** — Marginal Lending Facility Rate
- **All Key Rates** — Combined view
- **MFI Rates** — Bank lending/deposit rates


## Available Tools
- **get_key_rates**: This is the rate at which banks can borrow from the ECB for one week. It's the most important eurozone interest rate for monetary policy.

Get the ECB's key interest rates — the main refinancing rate (MRO)
- **get_deposit_rate**: Since October 2019, this has become the most closely watched ECB rate as it effectively determines the lower bound of money market rates.

Get the ECB deposit facility rate — the floor of the interest rate corridor
- **get_marginal_lending_rate**: Forms the upper bound of the ECB's interest rate corridor.

Get the ECB marginal lending facility rate — the ceiling of the rate corridor
- **get_all_key_rates**: Shows the full rate corridor.

Get all 3 ECB key interest rates together: MRO, deposit, and marginal lending
- **get_mfi_rates**: Shows what banks actually charge/pay for loans and deposits. Key indicator of monetary policy transmission.

Get MFI interest rates — bank lending and deposit rates in the eurozone


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ECB Interest Rates — Monetary Policy Rates & Banking** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the current ECB interest rates?"

**🤖 AI Agent:**
> 🏦 **ECB Key Interest Rates**

| Rate | Current | Previous |
|------|---------|----------|
| Deposit Facility (DFR) | 2.50% | 2.75% |
| Main Refinancing (MRO) | 2.65% | 2.90% |
| Marginal Lending (MLFR) | 2.90% | 3.15% |

Last decision: 6 March 2026 (cut by 25bp)
Next meeting: 17 April 2026

---

**👤 You:**
> "Fetch the latest Marginal Lending Facility Rate."

**🤖 AI Agent:**
> The latest Marginal Lending Facility Rate (MLFR) is currently standing at 2.90%. This rate defines the ceiling for the overnight interest rates in the banking system.

---

**👤 You:**
> "Show the difference between the MRO and the DFR."

**🤖 AI Agent:**
> The current spread between the Main Refinancing Operations (MRO) rate and the Deposit Facility Rate (DFR) is 15 basis points. The MRO is at 2.65% while the DFR is at 2.50%.


## ❓ FAQ

**Q: What is the difference between MRO and DFR?**
MRO (Main Refinancing Operations) is the rate at which banks can borrow from the ECB for one week. DFR (Deposit Facility Rate) is the rate banks earn on overnight deposits. Since 2019, DFR has become the de facto benchmark for money markets in the eurozone.

**Q: Does this server also track commercial bank interest rates?**
Yes, it provides access to MFI (Monetary Financial Institutions) lending and deposit rates, which reflect the commercial banks' rates passed on to households and non-financial corporations.

**Q: Are the rates updated immediately after the ECB Governing Council decisions?**
Yes, the official policy rates (MRO, DFR, MLFR) are updated in the ECB's Statistical Data Warehouse generally very shortly after the official announcement by the Governing Council.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecb-interest-rates-monetary-policy-rates-banking](https://vinkius.com/mcp/ecb-interest-rates-monetary-policy-rates-banking)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ECB Interest Rates — Monetary Policy Rates & Banking** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ecb-interest-rates-monetary-policy-rates-banking` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ECB Interest Rates — Monetary Policy Rates & Banking** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecb-interest-rates-monetary-policy-rates-banking": {
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
