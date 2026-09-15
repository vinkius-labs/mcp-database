# Convertible Note Conversion Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/convertible-note-conversion-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate conversion shares, effective price, and equity ownership for convertible notes.

## Description
This MCP server provides precise financial modeling for convertible note conversions. It allows AI agents to calculate conversion shares, effective price per share, and investor equity percentage by analyzing principal, interest, valuation caps, and discount rates. Use `get_conversion_summary` for single notes, `calculate_mfn_adjustment` to evaluate Most Favored Nation clauses, `aggregate_multiple_notes` to sum the impact of several notes, and `compare_scenarios` to model different financing outcomes.


## Available Tools (4)
- **aggregate_multiple_notes**: Calculates the combined impact of multiple convertible notes converting simultaneously
- **calculate_mfn_adjustment**: Determines if a note holder should switch to more favorable terms based on an MFN clause
- **compare_scenarios**: Evaluates the difference in equity ownership between two different financing scenarios
- **get_conversion_summary**: Calculates the primary conversion metrics for a single convertible note


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Convertible Note Conversion Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the conversion for a $100,000 note with 5% interest, a $5,000,000 valuation cap, a 20% discount, and a next round price of $1.00 with 10,000,000 pre-money shares."

**🤖 AI Agent:**
> The total conversion amount is $105,000. With a cap price of $0.50 and a discount price of $0.80, the conversion price is $0.50. This results in 210,000 conversion shares and an equity percentage of 2.05%.

---

**👤 You:**
> "Compare two scenarios: Scenario A has a $4M cap and Scenario B has a $6M cap, both with a 20% discount and $1.00 next round price, given 10,000,000 pre-money shares."

**🤖 AI Agent:**
> Scenario A results in a higher equity stake due to the lower valuation cap. The equity delta between the two scenarios is 0.55%.

---

**👤 You:**
> "I have a note with a $5M cap and 10% discount. A new note is issued with a $4M cap and 15% discount. Should I switch terms?"

**🤖 AI Agent:**
> Yes, switching to the new terms is more favorable as both the valuation cap is lower and the discount rate is higher.


## ❓ FAQ

**Q: How does the valuation cap affect my conversion?**
The valuation cap sets a maximum price for your conversion. If the next round's valuation is higher than the cap, you convert at the lower cap price, securing more equity.

**Q: Can I calculate the impact of multiple notes at once?**
Yes, you can use `aggregate_multiple_notes` to calculate the total conversion shares and combined equity percentage for a group of notes converting in the same round.

**Q: What is an MFN clause?**
A Most Favored Nation (MFN) clause ensures that if a company issues new notes with better terms, the original note holder can adopt those improved terms using `calculate_mfn_adjustment`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/convertible-note-conversion-engine](https://vinkius.com/en/ai-agent-connect/convertible-note-conversion-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Convertible Note Conversion Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `convertible-note-conversion-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Convertible Note Conversion Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "convertible-note-conversion-engine": {
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
