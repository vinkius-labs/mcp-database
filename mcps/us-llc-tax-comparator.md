# US LLC Tax Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-llc-tax-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare federal and state tax liabilities across different US business entity structures.

## Description
This MCP server provides AI agents with the ability to perform detailed tax liability comparisons for US-based businesses. By using tools like `calculate_tax_comparison`, `evaluate_s_corp_savings_potential`, and `get_state_tax_context`, an agent can analyze how different entity structures--such as Sole Proprietorship, Partnership, S-Corp, and C-Corp--impact total tax burdens based on annual profit, owner salary, and state jurisdiction. This is essential for financial planning and optimizing business structure elections.


## Available Tools (3)
- **calculate_tax_comparison**: Compare tax liabilities across different business structures
- **evaluate_s_corp_savings_potential**: Quantify potential tax savings from S-Corp election
- **get_state_tax_context**: Retrieve tax environment information for a specific state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US LLC Tax Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare taxes for a business with $150,000 profit and $60,000 salary in California."

**🤖 AI Agent:**
> Running `calculate_tax_comparison` for CA with $150k profit and $60k salary... [Detailed comparison result follows]

---

**👤 You:**
> "How much can I save by switching to an S-Corp if my profit is $200,000 and salary is $80,000 in Texas?"

**🤖 AI Agent:**
> Using `evaluate_s_corp_savings_potential` for TX... The analysis shows a potential net savings of [Calculated Amount].

---

**👤 You:**
> "What is the tax environment like in New York?"

**🤖 AI Agent:**
> Calling `get_state_tax_context` for NY... The estimated state income tax rate is [Rate] and it is classified as a [Tier] burden state.


## ❓ FAQ

**Q: How can I compare taxes for different business types?**
Use the `calculate_tax_comparison` tool by providing your annual profit, owner salary, and state code to see a side-by-side breakdown of liabilities.

**Q: Can I estimate the benefits of an S-Corp election?**
Yes. The `evaluate_s_corp_savings_potential` tool specifically calculates the potential net savings and percentage reduction in tax burden.

**Q: Does the tool account for state-specific taxes?**
Yes, by using `get_state_tax_context` or providing a `stateCode` to other tools, the server retrieves relevant state income tax rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-llc-tax-comparator](https://vinkius.com/mcp/us-llc-tax-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US LLC Tax Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-llc-tax-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US LLC Tax Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-llc-tax-comparator": {
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
