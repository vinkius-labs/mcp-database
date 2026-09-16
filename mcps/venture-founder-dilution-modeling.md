# Venture Founder Dilution Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-founder-dilution-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Model founder ownership, dilution, and exit proceeds through successive funding rounds.

## Description
This MCP server provides a suite of tools to model the complex lifecycle of founder equity. Use `simulate_dilution_rounds` to track ownership changes through multiple funding rounds and option pool refreshes. Calculate final payouts with `calculate_exit_outcomes` and evaluate long-term sustainability using `assess_founder_motivation`. It also provides a high-level overview of equity loss via `get_dilution_summary`.


## Available Tools (4)
- **simulate_dilution_rounds**: Calculates the step-by-step ownership percentage of founders through a sequence of funding rounds and option pool refreshes
- **calculate_exit_outcomes**: Determines the financial outcome for the founder at a specific exit event
- **get_dilution_summary**: Provides a high-level overview of the total dilution experienced by the founder
- **assess_founder_motivation**: Evaluates if the projected financial outcome is high enough to sustain founder interest


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Founder Dilution Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I started with 100% ownership. I had a Seed round with $1M pre-money and $200k investment, and a 10% option pool refresh. What is my ownership after this round?"

**🤖 AI Agent:**
> After the Seed round and the 10% option pool refresh, your ownership is 72.73%.

---

**👤 You:**
> "If I own 15% of a company and it exits for $50,000,000, how much will I receive?"

**🤖 AI Agent:**
> You will receive $7,500,000 upon exit.

---

**👤 You:**
> "I have 5% ownership and my exit proceeds are $100,000. How is my motivation assessed?"

**🤖 AI Agent:**
> The motivation score is low because the exit proceeds are insufficient relative to the ownership percentage.


## ❓ FAQ

**Q: How does an option pool refresh affect my ownership?**
An option pool refresh dilutes all existing shareholders, including founders and previous investors, to ensure the new pool meets the target percentage of the post-money valuation.

**Q: Can I model multiple funding rounds at once?**
Yes, you can use `simulate_dilution_rounds` by providing an array of funding rounds, each containing a pre-money valuation and an investment amount.

**Q: What is the difference between pre-money and post-money valuation?**
Pre-money valuation is the value of the company before the new investment is added. Post-money valuation is the sum of the pre-money valuation and the new investment amount.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-founder-dilution-modeling](https://vinkius.com/en/ai-agent-connect/venture-founder-dilution-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Founder Dilution Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-founder-dilution-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Founder Dilution Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-founder-dilution-modeling": {
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
