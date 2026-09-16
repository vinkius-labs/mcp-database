# Venture Closing Conditions Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-closing-conditions-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze M&A deal timelines, critical paths, and closing probabilities.

## Description
This MCP server provides strategic tools for analyzing M&A or venture capital deal timelines. It helps identify bottleneck dependencies and assess the likelihood of meeting target closing dates. Use `analyze_closing_timeline` to determine the total estimated time and critical path, `calculate_satisfaction_probability` to assess the statistical likelihood of success, `evaluate_party_responsibilities` to identify friction points between stakeholders, and `check_regulatory_and_third_party_impact` to isolate the impact of external entities like regulators or landlords.


## Available Tools (4)
- **analyze_closing_timeline**: Determine the total estimated time required to close the deal and identify delaying items
- **calculate_satisfaction_probability**: Assess the statistical likelihood of meeting the target closing date
- **check_regulatory_and_third_party_impact**: Isolate and analyze the impact of external entities on deal velocity
- **evaluate_party_responsibilities**: Break down party responsibilities to identify potential friction points


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Closing Conditions Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated closing timeline for my deal with these conditions: { name: 'Regulatory Approval', durationWeeks: 4, dependencies: [] }, { name: 'Buyer Board Approval', durationWeeks: 2, dependencies: ['Regulatory Approval'] }?"

**🤖 AI Agent:**
> The estimated closing timeline is 6 weeks, with 'Buyer Board Approval' being a critical path item.

---

**👤 You:**
> "What is the probability of closing on time if I have a high-risk regulatory condition and the total duration is 8 weeks?"

**🤖 AI Agent:**
> The probability of meeting the target date is 65%, with the primary risk driver being the high-risk regulatory requirement.

---

**👤 You:**
> "Which party is responsible for the most work in this deal?"

**🤖 AI Agent:**
> The Seller is the bottleneck party, as they hold the highest cumulative duration of active tasks in the critical path.


## ❓ FAQ

**Q: How do I calculate the estimated closing timeline?**
You can use the `analyze_closing_timeline` tool by providing an array of conditions with their durations and dependencies.

**Q: Can I assess the risk of missing a closing date?**
Yes, the `calculate_satisfaction_probability` tool assesses the statistical likelihood of meeting your target date based on condition complexity.

**Q: How are external delays handled?**
The `check_regulatory_and_third_party_impact` tool specifically isolates and analyzes the impact of regulatory and third-party requirements on deal velocity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-closing-conditions-checklist](https://vinkius.com/en/ai-agent-connect/venture-closing-conditions-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Closing Conditions Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-closing-conditions-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Closing Conditions Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-closing-conditions-checklist": {
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
