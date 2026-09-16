# Wine Nitrogen Requirement Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-nitrogen-requirement-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate yeast assimilable nitrogen (YAN) needs and precision supplementation strategies.

## Description
This MCP server provides enologists with precise tools to manage yeast nutrition during fermentation. Use `calculate_yan_deficit` to determine if current nitrogen levels meet the requirements of your specific yeast strain and sugar concentration. For immediate needs, `plan_dap_supplementation` generates a safe, staged addition schedule for inorganic nitrogen. For long-term yeast health, `optimize_organic_strategy` provides a nutritional plan using organic sources, while `evaluate_fermentation_risk` offers a qualitative assessment of potential stuck fermentations or H2S production risks.


## Available Tools (4)
- **calculate_yan_deficit**: Determines if the current nitrogen levels are sufficient for the planned fermentation
- **evaluate_fermentation_risk**: Provides a qualitative assessment of the risk of stuck fermentation or H2S production
- **optimize_organic_strategy**: Provides a long-term nutritional plan using organic nitrogen sources
- **plan_dap_supplementation**: Calculates the specific amount and timing for inorganic nitrogen (DAP) additions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Nitrogen Requirement Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the YAN deficit for a must with 24 Brix, 150 mg/L initial YAN, and a strain demand factor of 1.2."

**🤖 AI Agent:**
> The required YAN is 288 mg/L, resulting in a deficit of 138 mg/L.

---

**👤 You:**
> "What is the risk level for a fermentation with 100 mg/L YAN and 25 Brix using a strain factor of 1.5?"

**🤖 AI Agent:**
> The risk level is High due to High Sugar Demand.

---

**👤 You:**
> "Plan a DAP supplementation for a 50 mg/L deficit over a 7-day fermentation with a target rate of 1.0."

**🤖 AI Agent:**
> Total DAP needed is 50 mg/L. The schedule is: Day 1: 25 mg/L, Day 3: 15 mg/L, Day 5: 10 mg/L.


## ❓ FAQ

**Q: How do I know if my nitrogen levels are sufficient?**
You can use the `calculate_yan_deficit` tool. By providing the initial Brix, current YAN, and the yeast strain demand factor, the tool will tell you if your levels are sufficient or if a deficit exists.

**Q: Can this tool help prevent stuck fermentations?**
Yes. By using `evaluate_fermentation_risk` and `plan_dap_supplementation`, you can identify high-risk scenarios and create a controlled nitrogen addition schedule to support yeast health and prevent stalls.

**Q: What is the difference between DAP and organic supplementation?**
DAP is an inorganic source used for rapid nitrogen boosts via `plan_dap_supplementation`. Organic sources, managed through `optimize_organic_strategy`, provide a more gradual and sustained nutritional profile for long-term yeast vitality.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-nitrogen-requirement-calculator](https://vinkius.com/en/ai-agent-connect/wine-nitrogen-requirement-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Nitrogen Requirement Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-nitrogen-requirement-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Nitrogen Requirement Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-nitrogen-requirement-calculator": {
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
