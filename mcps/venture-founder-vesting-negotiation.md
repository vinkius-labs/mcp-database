# Venture Founder Vesting Negotiation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-founder-vesting-negotiation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Models optimal founder vesting terms by balancing equity retention and investor protection.

## Description
This MCP server provides a negotiation modeling engine to simulate founder vesting structures. It calculates recommended terms, flexibility ranges, and the balance between investor protection and founder incentives. Use `get_recommended_terms` to find balanced structures, `get_flexibility_range` to identify negotiation zones, `evaluate_protection_balance` to check term alignment, and `simulate_commitment_impact` to see how seniority affects vesting.


## Available Tools (4)
- **evaluate_protection_balance**: Analyzes whether the proposed terms favor the investor too heavily or the founder too heavily
- **get_flexibility_range**: Determines the "negotiation zone" for a founder to understand how much they can push back on investor demands
- **get_recommended_terms**: Provides the most balanced vesting structure based on the provided negotiation parameters
- **simulate_commitment_impact**: Models how changes in founder experience or commitment levels affect the suggested vesting structure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Founder Vesting Negotiation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the recommended vesting terms for a 48-month schedule with a 12-month cliff, single-trigger acceleration, a leverage of 5, and experience of 8?"

**🤖 AI Agent:**
> The recommended cliff is 12 months, the recommended acceleration is single-trigger, and the recommended schedule is 48 months, with a high founder incentive score.

---

**👤 You:**
> "What is my negotiation flexibility for a 36-month schedule with a leverage of 7?"

**🤖 AI Agent:**
> Your negotiation zone allows for a cliff between 3 and 9 months and a schedule between 30 and 42 months.

---

**👤 You:**
> "Is my proposed 60-month schedule with a 24-month cliff and no acceleration fair?"

**🤖 AI Agent:**
> The proposed terms favor the investor heavily, resulting in a high investor protection level and a low founder incentive level.


## ❓ FAQ

**Q: How can I find the best vesting schedule for my startup?**
You can use the `get_recommended_terms` tool to generate a balanced vesting structure based on your specific parameters like schedule length and founder leverage.

**Q: What is a 'cliff' in vesting?**
A cliff is a probationary period at the start of a vesting schedule. No equity is earned until this period expires.

**Q: Can I see how my experience affects my negotiation power?**
Yes, the `simulate_commitment_impact` tool allows you to model how changes in experience or commitment levels affect the suggested vesting structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-founder-vesting-negotiation](https://vinkius.com/en/ai-agent-connect/venture-founder-vesting-negotiation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Founder Vesting Negotiation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-founder-vesting-negotiation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Founder Vesting Negotiation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-founder-vesting-negotiation": {
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
