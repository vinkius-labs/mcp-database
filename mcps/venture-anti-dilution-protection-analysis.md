# Venture Anti-Dilution Protection Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-anti-dilution-protection-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze the impact of anti-dilution protection mechanisms during down-rounds.

## Description
This MCP server provides specialized tools to model the impact of anti-dilution provisions on investor ownership. It allows for precise calculations of how different protection mechanisms affect share counts and ownership percentages when a company undergoes a down-round. Use `calculate_full_ratchet_impact` for aggressive protection modeling, `calculate_weighted_average_impact` for standard market scenarios, `analyze_shareholder_dilution` to evaluate the impact on non-protected holders, or `compare_protection_mechanisms` to see the difference between methods.


## Available Tools (4)
- **analyze_shareholder_dilution**: Evaluates how the anti-dilution adjustment affects the ownership percentages of non-protected shareholders
- **calculate_weighted_average_impact**: Calculates the impact of a broad-based weighted average anti-dilution adjustment
- **compare_protection_mechanisms**: Directly compares the severity of Full Ratchet versus Weighted Average for a specific scenario
- **calculate_full_ratchet_impact**: Calculates the specific impact of a full ratchet anti-dilution adjustment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Anti-Dilution Protection Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the impact of a full ratchet adjustment if an investor put in $1,000,000 at $10 per share, and the new down-round price is $5 per share with 1,000,000 shares outstanding."

**🤖 AI Agent:**
> Under a full ratchet adjustment, the investor would receive 200,000 additional shares, resulting in a new adjusted conversion price of $5.00.

---

**👤 You:**
> "Compare full ratchet vs weighted average for a $500,000 investment at $20/share, with a down-round at $15/share, $2,000,000 new capital raised, and 5,000,000 shares outstanding."

**🤖 AI Agent:**
> The full ratchet method would issue 16,666 additional shares, while the weighted average method would issue 11,111 additional shares, a difference of 5,555 shares.

---

**👤 You:**
> "If non-protected shareholders own 80% of the company (0.80) and 50,000 new shares are issued to a protected investor, what is the impact on the non-protected ownership if there were 500,000 total shares before?"

**🤖 AI Agent:**
> The non-protected ownership will be diluted from 80% to 76.19% due to the issuance of the 50,000 new shares.


## ❓ FAQ

**Q: What is the difference between Full Ratchet and Weighted Average?**
Full Ratchet is the most aggressive protection, adjusting the conversion price to the new lower price regardless of the amount raised. Broad-Based Weighted Average is more moderate, adjusting the price based on both the new price and the amount of capital raised relative to existing shares.

**Q: How can I compare the two main protection methods?**
You can use the `compare_protection_mechanisms` tool to see a side-by-side comparison of the additional shares issued under both Full Ratchet and Weighted Average for your specific scenario.

**Q: Does this tool account for dilution of other shareholders?**
Yes, the `analyze_shareholder_dilution` tool specifically calculates how the issuance of new shares to protected investors impacts the ownership percentages of all non-protected shareholders.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-anti-dilution-protection-analysis](https://vinkius.com/en/ai-agent-connect/venture-anti-dilution-protection-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Anti-Dilution Protection Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-anti-dilution-protection-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Anti-Dilution Protection Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-anti-dilution-protection-analysis": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
