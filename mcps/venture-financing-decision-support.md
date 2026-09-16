# Venture Financing Decision Support MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-financing-decision-support)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Compare the economic and legal impact of priced rounds versus convertible instruments.

## Description
This MCP server provides a suite of decision-support tools for founders and investors to evaluate financing options. Use `compare_financing_economics` to determine ownership impact and dilution, `analyze_execution_friction` to evaluate legal costs and closing timelines, and `evaluate_investor_protections` to assess the impact of specific investor rights. Finally, use `generate_strategic_recommendation` to receive a data-driven decision based on economic, friction, and protection models.


## Available Tools (4)
- **analyze_execution_friction**: Evaluates the time and financial costs required to close each type of round
- **compare_financing_economics**: Compares the direct ownership impact and dilution for both priced rounds and convertible instruments
- **evaluate_investor_protections**: Assesses how different rights affect the attractiveness of the round
- **generate_strategic_recommendation**: Provides a final decision based on the combined economic, friction, and protection data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Financing Decision Support** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare a $500,000 investment at a $4M pre-money valuation against a SAFE with a $5M cap."

**🤖 AI Agent:**
> The priced round results in 11.11% dilution for the founder, while the convertible instrument with a $5M cap results in 10% dilution, providing a 1.11% ownership advantage to the founder.

---

**👤 You:**
> "What is the cost difference if a priced round costs $50,000 and takes 8 weeks, while a convertible round costs $5,000 and takes 2 weeks?"

**🤖 AI Agent:**
> The priced round carries a $45,000 higher legal cost and takes 6 weeks longer to close than the convertible round.

---

**👤 You:**
> "I have high leverage (score 8). Should I use a priced round or a convertible instrument?"

**🤖 AI Agent:**
> Given your high founder leverage, a convertible instrument with a high valuation cap is recommended to minimize immediate dilution and reduce legal friction.


## ❓ FAQ

**Q: How do I compare dilution between a priced round and a SAFE?**
You can use the `compare_financing_economics` tool. Provide the investment amount, pre-money valuation, and the valuation cap or discount rate for the convertible instrument to see the ownership delta.

**Q: Can this tool help me estimate legal costs?**
Yes, the `analyze_execution_friction` tool allows you to input estimated legal fees and timelines for both priced rounds and convertible rounds to compare the total cost and efficiency.

**Q: What factors influence the final recommendation?**
The `generate_strategic_recommendation` tool synthesizes data from economics, friction, and protection analyses, while also accounting for your specific founder leverage score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-financing-decision-support](https://vinkius.com/en/ai-agent-connect/venture-financing-decision-support)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Financing Decision Support** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-financing-decision-support` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Financing Decision Support** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-financing-decision-support": {
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
