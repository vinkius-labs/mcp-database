# Underground Mining Method Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/underground-mining-method-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Evaluates geological parameters to recommend optimal underground mining methods.

## Description
This MCP server provides decision-support tools for mining engineers to select the most efficient underground mining approach. By analyzing ore body geometry, rock stability, and depth, it calculates suitability scores for methods like `block_caving` or `room_and_pillar`. It also includes safety checks via `validate_geotechnical_constraints` to ensure selected methods are viable under specific depth and rock strength conditions.


## Available Tools (4)
- **get_method_characteristics**: g., "room_and_pillar").

Retrieve technical properties and cost-profile of a specific mining method
- **get_mining_method_suitability**: Calculate suitability scores for all available mining methods based on site parameters
- **recommend_optimal_method**: Identify the single best mining approach from suitability scores
- **validate_geotechnical_constraints**: Check if depth and rock strength allow for safe mining methods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Underground Mining Method Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate suitability scores for an ore body with 20m thickness, 15 degree dip, 60 rock strength, 500m depth, and 2.5 grade."

**🤖 AI Agent:**
> { "scores": { "room_and_pillar": 0.4, "sublevel_caving": 0.7, "block_caving": 0.8, "cut_and_fill": 0.3, "longwall": 0.5 }, "metadata": { "calculatedAt": "2024-05-20T10:00:00Z" } }

---

**👤 You:**
> "Which mining method is best for these scores: { "room_and_pillar": 0.4, "sublevel_caving": 0.7, "block_caving": 0.8, "cut_and_fill": 0.3, "longwall": 0.5 }?"

**🤖 AI Agent:**
> { "recommendedMethod": "block_caving", "confidenceScore": 0.8, "reasoning": "Selected due to high ore thickness and low grade requirements." }

---

**👤 You:**
> "Is it safe to use room and pillar mining at 800m depth with a rock strength of 40?"

**🤖 AI Agent:**
> { "isSafe": false, "restrictedMethods": ["room_and_pillar"], "warningMessage": "High depth to rock strength ratio makes room and pillar unsafe." }


## ❓ FAQ

**Q: How does the tool determine the best mining method?**
The tool uses `get_mining_method_suitability` to calculate scores based on ore thickness, dip, rock strength, depth, and grade, then identifies the best option.

**Q: Can I check if a specific method is safe for my site?**
Yes, you can use `validate_geotechnical_constraints` to check if the depth and rock strength allow for safe operations.

**Q: What information is needed for suitability calculation?**
You need to provide the ore thickness, dip angle, rock strength index, mining depth, and ore grade.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/underground-mining-method-selector](https://vinkius.com/ai-agent-connect/underground-mining-method-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Underground Mining Method Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `underground-mining-method-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Underground Mining Method Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "underground-mining-method-selector": {
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
