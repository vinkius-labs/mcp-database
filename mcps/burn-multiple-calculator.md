# Burn Multiple Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/burn-multiple-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Evaluate SaaS growth efficiency by measuring capital expenditure against new ARR.

## Description
The Burn Multiple Calculator is a diagnostic tool for SaaS companies to assess their capital efficiency. By analyzing the relationship between net burn and net new ARR, it identifies whether your growth is efficient or concerning. Use `calculate_burn_efficiency` to determine your efficiency tier, `compare_to_benchmark` to see how you stack up against the Bessemer Cloud Index, or `get_growth_audit` for a comprehensive health check of your company's performance.


## Available Tools (3)
- **compare_to_benchmark**: Compare burn multiple to industry benchmarks
- **calculate_burn_efficiency**: Lower is better.

Calculate the burn multiple efficiency
- **get_growth_audit**: Perform a full growth and efficiency audit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Burn Multiple Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I lost $500,000 in net burn and added $400,000 in new ARR. What is my efficiency tier?"

**🤖 AI Agent:**
> Your burn multiple is 1.25x, which places you in the Good efficiency tier.

---

**👤 You:**
> "My current burn multiple is 0.8. How does this compare to industry benchmarks?"

**🤖 AI Agent:**
> A burn multiple of 0.8x means you are Outperforming the industry standard benchmark.

---

**👤 You:**
> "Perform a growth audit for a company with $1,000,000 net burn and $600,000 new ARR."

**🤖 AI Agent:**
> The audit shows your burn multiple is 1.67x. This falls into the Reasonable tier, indicating you are currently Underperforming relative to the industry standard.


## ❓ FAQ

**Q: What is a Burn Multiple?**
A Burn Multiple measures how much cash a company burns to generate one unit of new Annual Recurring Revenue (ARR). A lower ratio indicates higher capital efficiency.

**Q: How do I interpret the results?**
The tool classifies efficiency into tiers: Excellent (below 1.0x), Good (1.0x-1.5x), Reasonable (1.5x-2.0x), and Concerning (above 2.0x).

**Q: Can I compare my metrics to industry standards?**
Yes, using the `compare_to_benchmark` tool, you can see if your burn multiple is outperforming or underperforming relative to the Bessemer Cloud Index standards.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/burn-multiple-calculator](https://vinkius.com/mcp/burn-multiple-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Burn Multiple Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `burn-multiple-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Burn Multiple Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "burn-multiple-calculator": {
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
