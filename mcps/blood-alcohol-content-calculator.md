# Blood Alcohol Content Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blood-alcohol-content-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Estimate BAC, legal limits, and impairment risks.

## Description
The Blood Alcohol Content Calculator provides precise estimations of your current blood alcohol concentration based on weight, gender, drinks consumed, and time elapsed. Use `calculate_bac_metrics` to find out how much time remains until you are sober, `get_jurisdiction_limit` to check legal driving thresholds in various US states and European countries, `get_impairment_details` to understand the physical effects of your current BAC level, and `analyze_medication_risk` to assess potential dangers when consuming alcohol while taking specific medications.


## Available Tools (4)
- **calculate_bac_metrics**: Calculate current BAC and time until sober
- **get_impairment_details**: Get impairment details for a specific BAC level
- **get_jurisdiction_limit**: g., USA-CA, UK).

Get the legal BAC limit for a specific location
- **analyze_medication_risk**: Analyze potential risks of alcohol interaction with medications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blood Alcohol Content Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 180 lbs, I am male, and I just finished a 500ml beer with 5% ABV about 2 hours ago. What is my current BAC and when will I be sober?"

**🤖 AI Agent:**
> Your estimated BAC is approximately 0.021. You are expected to reach a BAC of 0.00 in about 2.5 hours.

---

**👤 You:**
> "What is the legal driving limit in California?"

**🤖 AI Agent:**
> The legal BAC limit for driving in California (USA-CA) is 0.08%.

---

**👤 You:**
> "What are the physical symptoms of having a BAC of 0.15?"

**🤖 AI Agent:**
> At a BAC of 0.15, you may experience significant loss of coordination, impaired judgment, and slowed reaction times.


## ❓ FAQ

**Q: How accurate is the BAC estimation?**
The `calculate_bac_metrics` tool uses biological variables like weight and gender to provide a scientific estimate, though individual metabolism can vary.

**Q: Does the calculator account for food consumption?**
Yes, providing the `hasFoodInStomach` parameter helps simulate the delay in alcohol absorption into the bloodstream.

**Q: Can I check legal limits for specific countries?**
Yes, use `get_jurisdiction_limit` with a location name like 'Germany' or 'USA-CA' to retrieve the maximum allowable BAC threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blood-alcohol-content-calculator](https://vinkius.com/mcp/blood-alcohol-content-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blood Alcohol Content Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blood-alcohol-content-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blood Alcohol Content Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blood-alcohol-content-calculator": {
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
