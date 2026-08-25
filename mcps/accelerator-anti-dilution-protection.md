# Accelerator Anti-Dilution Protection MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-anti-dilution-protection)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the impact of anti-dilution provisions and pay-to-play rules on investor holdings.

## Description
This MCP server provides precise analytical tools for venture capital modeling. It allows investors and founders to calculate the exact impact of down-rounds on equity ownership. Use `calculate_anti_dilution_impact` to determine additional shares issued and adjusted ownership percentages. Use `compare_protection_methods` to evaluate the difference between Full Ratchet and Weighted Average adjustments. Additionally, `validate_pay_to_play_eligibility` helps determine if an investor maintains their rights based on participation thresholds.


## Available Tools (3)
- **calculate_anti_dilution_impact**: Calculates the impact of anti-dilution provisions on investor holdings
- **compare_protection_methods**: Compares the outcomes of Full Ratchet and Weighted Average anti-dilution methods
- **validate_pay_to_play_eligibility**: Validates if an investor is eligible for anti-dilution protection based on pay-to-play rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Anti-Dilution Protection** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the anti-dilution impact for an investor with 10,000 shares at $5.00 per share, if a down-round occurs at $3.00 with 5,000 new shares being issued using weighted average."

**🤖 AI Agent:**
> The investor will receive 2,500 additional shares, resulting in a total of 12,500 shares and an adjusted ownership of 12.5%.

---

**👤 You:**
> "Compare the impact of Full Ratchet vs Weighted Average for an investment of $1,000,000 with 100,000 shares at $10.00, given a down-round at $5.00 with 20,000 new shares."

**🤖 AI Agent:**
> Full Ratchet will issue 100,000 additional shares, whereas Weighted Average will issue significantly fewer shares. The delta in ownership is substantial.

---

**👤 You:**
> "Is an investor eligible for protection if they commit $50,000 to a $500,000 round where the requirement is 15% participation?"

**🤖 AI Agent:**
> No, the investor is not eligible. They committed 10% of the round, which is below the required 15% threshold, leaving a shortfall of $25,000.


## ❓ FAQ

**Q: What is the difference between Full Ratchet and Weighted Average?**
Full Ratchet resets the conversion price to the lowest price in the down-round, while Weighted Average adjusts the price based on the amount of capital raised at the new price.

**Q: How does pay-to-play affect my anti-dilution rights?**
If an investor fails to meet the required participation threshold in a new round, they may lose their anti-dilution protections entirely.

**Q: Can I use this with Claude Desktop?**
Yes, this server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-anti-dilution-protection](https://vinkius.com/ai-agent-connect/accelerator-anti-dilution-protection)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Anti-Dilution Protection** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-anti-dilution-protection` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Anti-Dilution Protection** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-anti-dilution-protection": {
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
