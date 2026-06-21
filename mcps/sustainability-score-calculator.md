# Sustainability Score Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sustainability-score-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Quantify your environmental footprint and discover actionable paths to a more sustainable lifestyle.

## Description
This MCP server provides AI agents with the ability to calculate personal sustainability scores based on daily habits. By using tools like `calculate_personal_score`, `get_category_status`, and `generate_improvement_roadmap`, agents can assess environmental impact across five key pillars: Transport, Food, Consumption, Energy, and Waste. The server processes raw habit data to return a weighted average score (0-100), qualitative assessments of each category, and personalized improvement roadmaps with actionable targets.


## Available Tools (3)
- **calculate_personal_score**: Returns weighted average and status.

Calculates the total sustainability score and provides a breakdown by category
- **generate_improvement_roadmap**: Provides personalized ecological goals and actionable targets
- **get_category_status**: Converts a numerical category score into a human-readable qualitative assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sustainability Score Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my sustainability score with a transport score of 80, food score of 60, and energy score of 40."

**🤖 AI Agent:**
> Your total sustainability score is 60. Your breakdown includes Transport (80), Food (60), and Energy (40).

---

**👤 You:**
> "What is the status of my energy usage if my score is 30?"

**🤖 AI Agent:**
> With an Energy score of 30, your impact level is Critical and urgent action is required.

---

**👤 You:**
> "Generate a roadmap to reach a target score of 90 based on my current scores: {'Transport': 70, 'Food': 50, 'Consumption': 60, 'Energy': 40, 'Waste': 55}."

**🤖 AI Agent:**
> To reach a target of 90, you should focus on improving your Energy and Food habits through the suggested actions in the roadmap.


## ❓ FAQ

**Q: How can an agent calculate my sustainability score?**
Agents use the `calculate_personal_score` tool, providing scores for categories like Transport, Food, and Energy to receive a total weighted average.

**Q: Can I get specific advice on improving my score?**
Yes. By using `generate_improvement_roadmap`, an agent can analyze your current breakdown and suggest actionable targets to reach a desired sustainability goal.

**Q: What categories are assessed?**
The assessment covers five pillars: Transport, Food, Consumption, Energy, and Waste. You can check the status of any specific pillar using `get_category_status`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sustainability-score-calculator](https://vinkius.com/mcp/sustainability-score-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sustainability Score Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sustainability-score-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sustainability Score Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sustainability-score-calculator": {
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
