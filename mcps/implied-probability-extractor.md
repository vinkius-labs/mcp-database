# Implied Probability Extractor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/implied-probability-extractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Convert American odds to true implied probability by removing the bookmaker margin.

## Description
The Implied Probability Extractor is a precision utility designed for bettors and analysts to strip the 'vig' (bookmaker margin) from American odds. By using tools like `get_true_probabilities`, `get_raw_probabilities`, and `calculate_overround_percentage`, you can reveal the underlying fair market probabilities of any sporting event. This allows you to identify value by comparing de-viggered probabilities against your own projections.


## Available Tools (3)
- **calculate_overround_percentage**: Determines the total margin (the "vig") being charged
- **get_raw_probabilities**: Converts American odds into unadjusted raw implied probabilities
- **get_true_probabilities**: Removes the bookmaker's margin to provide fair market probabilities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Implied Probability Extractor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the true probabilities for a game where the odds are -110 and +110?"

**🤖 AI Agent:**
> The true probability for both outcomes is 50.0%.

---

**👤 You:**
> "Calculate the overround for these odds: [-150, +130, +500]"

**🤖 AI Agent:**
> The total overround (vig) is 6.45%.

---

**👤 You:**
> "Convert these odds to raw probabilities: [-110, -110]"

**🤖 AI Agent:**
> The raw implied probabilities are 52.38% and 52.38%.


## ❓ FAQ

**Q: What is the 'vig' in betting?**
The 'vig', or vigorish, is the commission charged by a bookmaker to facilitate a bet. It is the margin built into the odds that ensures the house has an edge.

**Q: How do I find the fair probability of an outcome?**
You can use the `get_true_probabilities` tool. By providing the American odds for all possible outcomes, the tool removes the overround to show you the true, margin-free probability.

**Q: Can I check how much margin a bookmaker is charging?**
Yes, use the `calculate_overround_percentage` tool. It calculates the total market weight and shows you exactly how much the sum of probabilities exceeds 100%.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/implied-probability-extractor](https://vinkius.com/mcp/implied-probability-extractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Implied Probability Extractor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `implied-probability-extractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Implied Probability Extractor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "implied-probability-extractor": {
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
