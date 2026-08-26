# Sesame Seed Quality Grader MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sesame-seed-quality-grader)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [supply-chain](../categories/supply-chain.md)

Grade sesame seed quality, predict yields, and estimate market value.

## Description
This MCP server provides specialized tools for agricultural quality assessment of sesame seeds. It allows AI agents to determine commercial grade classifications using `grade_sesame_seeds`, estimate processed product outputs like oil and hulled seeds with `predict_yields`, calculate commercial pricing via `estimate_market_value`, and assess physical degradation using `analyze_harvest_impact`.


## Available Tools (4)
- **analyze_harvest_impact**: Evaluates how the specific harvest method has affected the seed's chemical and physical quality
- **estimate_market_value**: Calculates the commercial value of a seed batch based on quality metrics
- **grade_sesame_seeds**: Determines the commercial grade classification for a batch of seeds
- **predict_yields**: Estimates the potential output of processed products (hulled seeds and oil)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sesame Seed Quality Grader** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the grade for sesame seeds with 95 whiteness, 90 uniformity, 1% impurity, and 0.2% FFA?"

**🤖 AI Agent:**
> The sesame seeds are classified as Premium Export.

---

**👤 You:**
> "Predict the yields for seeds with 50% oil content, 85 uniformity, and mechanical harvesting."

**🤖 AI Agent:**
> The predicted hulled yield is 82% and the oil extraction yield is 44.5%.

---

**👤 You:**
> "Calculate the market value for USDA Grade A seeds with 52% oil content and 0.5% impurity."

**🤖 AI Agent:**
> The estimated value per unit is $4.50 with a quality premium of $0.75.


## ❓ FAQ

**Q: How does the grading tool work?**
The `grade_sesame_seeds` tool evaluates whiteness, uniformity, impurity, and FFA levels to assign a commercial grade like USDA Grade A or Premium Export.

**Q: Can I predict oil extraction yields?**
Yes, by using the `predict_yields` tool, you can estimate both the hulled seed yield and the volume of oil obtainable based on seed integrity and oil content.

**Q: Does harvest method affect the results?**
Yes, the `analyze_harvest_impact` tool specifically evaluates how different methods, such as mechanical vs manual, impact the seed's damage index and quality risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sesame-seed-quality-grader](https://vinkius.com/ai-agent-connect/sesame-seed-quality-grader)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sesame Seed Quality Grader** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sesame-seed-quality-grader` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sesame Seed Quality Grader** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sesame-seed-quality-grader": {
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
