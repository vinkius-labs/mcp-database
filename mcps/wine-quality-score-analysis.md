# Wine Quality Score Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-quality-score-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [statistics](../categories/statistics.md)

Statistical analysis of sensory evaluation scores for wine quality.

## Description
This MCP server provides statistical tools to analyze sensory evaluation data from wine tasting panels. It helps researchers and quality control teams understand wine quality through mean scores, assess panel reliability via agreement metrics, and verify the panel's ability to distinguish between samples. Use `get_wine_summary` to see average scores, `evaluate_panel_consistency` to check panelist agreement, `detect_discriminant_capability` to verify sample distinction, and `identify_panelist_outliers` to find biased scorers.


## Available Tools (4)
- **identify_panelist_outliers**: Finds panelists whose scoring behavior deviates significantly from the group norm
- **detect_discriminant_capability**: Checks if the panel is actually capable of telling the wines apart
- **evaluate_panel_consistency**: Determines how well the panelists agree with one another
- **get_wine_summary**: Provides a high-level overview of the mean quality scores for all wines in the dataset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Quality Score Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the average quality scores for all the wines in this dataset."

**🤖 AI Agent:**
> The average scores are: Cabernet Sauvignon: 8.2, Merlot: 7.5, and Pinot Noir: 7.9.

---

**👤 You:**
> "Is the tasting panel capable of distinguishing between these different wines?"

**🤖 AI Agent:**
> Yes, the panel has high discriminant power, showing significant differences between the wine varieties.

---

**👤 You:**
> "Are there any panelists providing biased scores?"

**🤖 AI Agent:**
> Panelist ID P-402 has been identified as an outlier due to a high deviation score.


## ❓ FAQ

**Q: What kind of data does this server process?**
It processes sensory evaluation scores, including wine IDs, panelist IDs, and numerical scores assigned during tastings.

**Q: How can I identify if my tasting panel is reliable?**
You can use the `evaluate_panel_consistency` tool to calculate agreement coefficients and determine if the panel's scoring is consistent.

**Q: Can I find panelists who are scoring inconsistently?**
Yes, the `identify_panelist_outliers` tool detects panelists whose scoring behavior deviates significantly from the group norm.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-quality-score-analysis](https://vinkius.com/en/ai-agent-connect/wine-quality-score-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Quality Score Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-quality-score-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Quality Score Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-quality-score-analysis": {
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
