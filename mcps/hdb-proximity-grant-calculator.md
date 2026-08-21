# HDB Proximity Grant Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/hdb-proximity-grant-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact HDB Proximity Housing Grant (PHG) amounts based on family ties and flat type.

## Description
This MCP server provides deterministic tools to calculate the Singapore HDB Proximity Housing Grant (PHG). It determines eligibility and exact grant amounts based on whether you are living with parents or living near them (within 4km), as well as the specific HDB flat type selected. Use `calculate_phg_grant` to get a full eligibility report or `validate_proximity_distance` to check if a location meets the proximity radius requirement.


## Available Tools (3)
- **calculate_phg_grant**: Determines the exact grant amount and eligibility for an applicant based on their proximity and flat type
- **get_flat_type_tier**: Categorizes the flat type into its respective grant tier for the "living near" rule
- **validate_proximity_distance**: Checks if a provided distance satisfies the proximity requirement for the "living near" grant tier


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HDB Proximity Grant Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much grant can I get if I am living with my parents in a 4-room flat?"

**🤖 AI Agent:**
> You are eligible for a grant of 30,000 SGD.

---

**👤 You:**
> "I live 3km away from my parents and I am buying a 3-room flat. What is my grant?"

**🤖 AI Agent:**
> You are eligible for a grant of 30,000 SGD.

---

**👤 You:**
> "What happens if I live 5km away from my parents and want to live near them in a 2-room flat?"

**🤖 AI Agent:**
> You are ineligible for the grant because the distance exceeds the 4km limit.


## ❓ FAQ

**Q: How is the grant amount determined?**
The grant amount depends on your family ties (living with or near parents) and the size of your flat. You can use `calculate_phg_grant` to see the specific amount for your situation.

**Q: What is the maximum distance allowed for the 'living near' grant?**
To qualify for the 'living near' tier, the distance must be 4km or less. The `validate_proximity_distance` tool can verify this for you.

**Q: Does the flat type affect the grant amount?**
Yes, for those living near parents, the grant amount scales with the flat type: 2-room flats receive 20,000 SGD, 3-room receive 30,000 SGD, and 4-room or larger receive 40,000 SGD.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/hdb-proximity-grant-calculator](https://vinkius.com/ai-agent-connect/hdb-proximity-grant-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HDB Proximity Grant Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hdb-proximity-grant-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HDB Proximity Grant Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hdb-proximity-grant-calculator": {
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
