# BTO Affordability Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bto-affordability-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate HDB BTO affordability, grants, and savings timelines.

## Description
This MCP server provides deterministic financial calculations for young Singaporean couples planning to purchase HDB Build-To-Order (BTO) flats. It connects AI agents to critical HDB eligibility logic, allowing them to determine if a couple qualifies for specific flat types using `validate_income_ceiling`. The server calculates the Enhanced CPF Housing Grant (EHG) via `check_grant_qualification` and provides a complete financial profile, including loan eligibility and years required to save for a downpayment, through `calculate_bto_eligibility`.


## Available Tools (3)
- **calculate_bto_eligibility**: Determine if a couple qualifies for a specific flat type and calculate their full affordability profile
- **check_grant_qualification**: Verify how much grant assistance a couple can receive
- **validate_income_ceiling**: Check if a specific flat type is accessible based on income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BTO Affordability Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can a couple earning 12,000 SGD monthly afford a 4-room BTO priced at 500,000 SGD?"

**🤖 AI Agent:**
> Based on the calculation, the couple is eligible for a 4-room flat. With an estimated grant and CPF savings, the remaining downpayment can be covered in approximately 3.5 years given their monthly savings.

---

**👤 You:**
> "Check if we qualify for a 5-room flat with a combined income of 22,000 SGD."

**🤖 AI Agent:**
> No, the combined income of 22,000 SGD exceeds the 21,000 SGD limit for 5-room flats in non-mature estates.

---

**👤 You:**
> "How much grant can a 30-year-old couple with 6,000 SGD monthly income receive?"

**🤖 AI Agent:**
> The couple is eligible for an Enhanced CPF Housing Grant of 80,000 SGD.


## ❓ FAQ

**Q: How is the income ceiling checked?**
The `validate_income_ceiling` tool ensures that the combined monthly income does not exceed the limits for the selected flat type, such as 14,000 SGD for 4-room flats.

**Q: Can I check my grant eligibility specifically?**
Yes, you can use the `check_grant_qualification` tool to isolate and calculate the Enhanced CPF Housing Grant (EHG) based on age and income.

**Q: What information is needed for a full affordability profile?**
To get a complete profile using `calculate_bto_eligibility`, you need the combined monthly income, age, first-timer status, target flat type, flat price, CPF OA savings, and monthly savings amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bto-affordability-index](https://vinkius.com/ai-agent-connect/bto-affordability-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BTO Affordability Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bto-affordability-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BTO Affordability Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bto-affordability-index": {
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
