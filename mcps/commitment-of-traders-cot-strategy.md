# Commitment of Traders (COT) Strategy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/commitment-of-traders-cot-strategy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze commercial and non-commercial positioning to generate deterministic trading signals.

## Description
This MCP server provides advanced algorithmic analysis of Commitment of Traders (COT) reports. It bridges the gap between raw commodity positioning data and actionable trading intelligence. By utilizing `analyze_cot_positioning`, users can calculate Z-scores, speculative sentiment, and hedging ratios. The `generate_trading_signal` tool applies strict deterministic rules to identify high-conviction BUY and SELL signals based on 'Smart Money' (Commercial) and 'Speculator' (Non-Commercial) positioning relative to price action and historical extremes. Finally, `get_signal_summary` provides a human-readable breakdown of all metrics and decisions.


## Available Tools (3)
- **analyze_cot_positioning**: Calculates core statistical metrics and sentiment indicators for a COT reporting period
- **get_signal_summary**: Formats the final signal output into a human-readable summary
- **generate_trading_signal**: Determines the exact trade direction (BUY, SELL, or HOLD)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Commitment of Traders (COT) Strategy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the current COT positioning for Gold using these metrics: commercial net 5000, non-commercial net -2000, Z-score 2.5, price 2050, 50-day MA 2000, net change 6000, days since report 1, and open interest 60000."

**🤖 AI Agent:**
> BUY signal with HIGH conviction. Commercials are heavily long (Z-score 2.5) and price is trending above the 50-day moving average.

---

**👤 You:**
> "Calculate the statistical metrics for this COT data: commercial long 10000, commercial short 5000, non-commercial long 8000, non-commercial short 2000, open interest 55000, and historical mean 0 with std dev 1000."

**🤖 AI Agent:**
> Commercial Net: 5000, Non-Commercial Net: 6000, Z-Score: 5.0, Speculative Sentiment: 10.9%, Hedging Ratio: 0.5, Divergence: False.

---

**👤 You:**
> "Generate a summary for a SELL signal where commercial net is -4000, non-commercial net is 7000, Z-score is 2.2, signal is SELL, and conviction is MEDIUM."

**🤖 AI Agent:**
> Signal: SELL | Conviction: MEDIUM. Commercial Net: -4000, Non-Commercial Net: 7000, Z-Score: 2.2. Speculators are extremely long, creating a contrarian sell opportunity.


## ❓ FAQ

**Q: What is the difference between Commercial and Non-Commercial signals?**
Commercial participants are hedgers (Smart Money) whose positioning often signals fundamental shifts. Non-Commercials are speculators whose extreme positioning often serves as a contrarian indicator.

**Q: How are BUY signals generated?**
A BUY signal is triggered when `commercialNet` is positive, the `cotZScore` exceeds 2.0, and the current price is above the 50-day moving average.

**Q: Does this tool support real-time data?**
The tool processes the COT data provided in the input. To ensure accuracy, the strategy includes a filter to ignore signals if the report is older than 3 days.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/commitment-of-traders-cot-strategy](https://vinkius.com/ai-agent-connect/commitment-of-traders-cot-strategy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Commitment of Traders (COT) Strategy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `commitment-of-traders-cot-strategy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Commitment of Traders (COT) Strategy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "commitment-of-traders-cot-strategy": {
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
