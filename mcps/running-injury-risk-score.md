# Running Injury Risk Score MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/running-injury-risk-score)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculates running injury risk profiles using the RRI model.

## Description
This MCP server provides specialized analytical tools to assess running injury risk. Use `get_risk_score` to evaluate overall vulnerability based on training load and history, `analyze_biomechanics` to assess movement patterns, `get_environmental_load_impact` to understand how surfaces and footwear affect load, and `get_prevention_plan` to receive personalized mitigation strategies.


## Available Tools (4)
- **get_environmental_load_impact**: Assesses how external factors like surface and gear influence the current load
- **analyze_biomechanics**: Evaluates movement patterns to determine their contribution to injury risk
- **get_prevention_plan**: Generates a set of personalized recommendations based on the risk profile
- **get_risk_score**: Calculates the primary injury risk score and identifies specific high-risk factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Injury Risk Score** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my running injury risk if I ran 40km this week, usually run 30km, have had previous injuries, do 1 strength session a week, run on asphalt, and have worn shoes?"

**🤖 AI Agent:**
> Your injury risk score is 75 (High). High-risk factors include a high training load ratio, previous injuries, and worn footwear.

---

**👤 You:**
> "Analyze my running biomechanics: cadence is 165, ground contact time is 280ms, and I use a heel strike."

**🤖 AI Agent:**
> Your biomechanical risk contribution is moderate. Consider increasing your cadence to reduce ground contact time.

---

**👤 You:**
> "Give me a prevention plan for a high risk score of 80 with high training load and low strength training."

**🤖 AI Agent:**
> To mitigate risk, reduce your weekly mileage immediately and prioritize resistance training focusing on lower body stability.


## ❓ FAQ

**Q: What is the RRI model?**
The Running Risk Index (RRI) is a model that assesses how physiological and environmental stressors contribute to injury likelihood.

**Q: How accurate are the biomechanics recommendations?**
The `analyze_biomechanics` tool provides data-driven suggestions based on your cadence and ground contact time to help optimize movement.

**Q: Can I use this with Claude Desktop?**
Yes, you can connect this server to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/running-injury-risk-score](https://vinkius.com/en/ai-agent-connect/running-injury-risk-score)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Injury Risk Score** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-injury-risk-score` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Injury Risk Score** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-injury-risk-score": {
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
