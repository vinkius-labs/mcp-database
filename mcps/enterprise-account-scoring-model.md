# Enterprise Account Scoring Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-account-scoring-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm](../categories/crm.md)

Prioritize B2B accounts using firmographics, technographics, and intent signals.

## Description
This MCP server connects AI agents to a sophisticated scoring engine that evaluates B2B account readiness. By synthesizing firmographic profiles, technology stacks, real-time intent, and engagement history, it provides a unified priority score. Use `calculate_account_score` to get a normalized 0-100 score, `classify_account_tiers` to assign priority levels, `get_prioritized_account_list` to generate ranked outreach lists, and `analyze_intent_signals` to evaluate recent market interest.


## Available Tools (4)
- **calculate_account_score**: Computes a single, normalized priority score for a specific account based on all available data dimensions
- **classify_account_tiers**: Assigns a priority tier to an account based on its calculated score
- **analyze_intent_signals**: Evaluates recent external activity to determine the "readiness" of an account
- **get_prioritized_account_list**: Generates a ranked list of accounts for sales outreach, sorted by their priority and tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Account Scoring Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the priority score for account ACC-123?"

**🤖 AI Agent:**
> The priority score for account ACC-123 is 85.

---

**👤 You:**
> "Show me the top 5 Tier 1 accounts."

**🤖 AI Agent:**
> Here are the top 5 Tier 1 accounts: ACC-001 (Score: 95), ACC-005 (Score: 92), ACC-012 (Score: 89), ACC-009 (Score: 88), and ACC-022 (Score: 87).

---

**👤 You:**
> "Analyze the intent for account ACC-456 for the last 30 days."

**🤖 AI Agent:**
> Account ACC-456 has an intent score of 72 based on 5 recent signals, including high-frequency research into enterprise software solutions.


## ❓ FAQ

**Q: How is the account score calculated?**
The score is a weighted aggregate of firmographics, technographics, intent, and engagement data, resulting in a value between 0 and 100.

**Q: Can I filter the prioritized account list?**
Yes, you can use the `get_prioritized_account_list` tool to filter by a minimum tier or set a limit on the number of accounts returned.

**Q: What are intent signals?**
Intent signals are external indicators of interest, such as website visits or research activity, analyzed via `analyze_intent_signals` to determine account readiness.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-account-scoring-model](https://vinkius.com/ai-agent-connect/enterprise-account-scoring-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Account Scoring Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-account-scoring-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Account Scoring Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-account-scoring-model": {
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
