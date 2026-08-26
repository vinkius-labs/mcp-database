# Horse Body Condition Scoring MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/horse-body-condition-scoring)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate Henneke Body Condition Scores (BCS) and nutritional weight plans.

## Description
This MCP server provides professional tools for assessing equine health using the Henneke scale. Use `get_bcs_analysis` to calculate an overall body condition score and identify fat deposition patterns across anatomical landmarks like the neck crest, withers, and tailhead. You can also use `get_weight_plan_recommendation` to generate nutritional management plans based on current and target scores, or `list_breed_profiles` to view ideal BCS ranges for draft, stock, and light horse categories.


## Available Tools (4)
- **get_bcs_analysis**: Calculates the overall body condition score and identifies fat deposition patterns
- **get_weight_plan_recommendation**: Provides a nutritional management plan based on the current BCS
- **list_breed_profiles**: Retrieves the expected fat distribution characteristics and ideal BCS ranges for different horse breeds
- **validate_measurement_inputs**: Verifies that all anatomical measurements provided are within valid Henneke ranges


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Horse Body Condition Scoring** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the BCS for a draft horse with a neck crest of 7, withers fat of 6, shoulder fat of 5, ribs visibility of 4, loin condition of 7, and tailhead fat of 6."

**🤖 AI Agent:**
> The calculated overall BCS for this draft horse is 6.0, indicating a moderately fleshy condition with fat deposition primarily at the crest and tailhead.

---

**👤 You:**
> "What is the ideal BCS range for a light horse breed?"

**🤖 AI Agent:**
> Light horse breeds typically have an ideal BCS range between 4 and 5.

---

**👤 You:**
> "My horse has a current BCS of 3 and a target BCS of 5. It weighs 450kg. What is the recommendation?"

**🤖 AI Agent:**
> The recommendation is to gain weight. You should implement a nutritional plan to increase mass to reach the target score of 5.


## ❓ FAQ

**Q: What is the Henneke scale?**
The Henneke scale is a standardized 1-9 scoring system used to assess the amount of fat and muscle on a horse to determine its body condition.

**Q: How do I get a weight management plan?**
You can use the `get_weight_plan_recommendation` tool by providing the current BCS, the target BCS for the specific breed, and the horse's current weight.

**Q: Does the scoring account for different horse breeds?**
Yes, the `get_bcs_analysis` tool adjusts its interpretation based on the breed type (draft, stock, or light) to account for varying fat distribution patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/horse-body-condition-scoring](https://vinkius.com/ai-agent-connect/horse-body-condition-scoring)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Horse Body Condition Scoring** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `horse-body-condition-scoring` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Horse Body Condition Scoring** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "horse-body-condition-scoring": {
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
