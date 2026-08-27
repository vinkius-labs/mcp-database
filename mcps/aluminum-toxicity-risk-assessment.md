# Aluminum Toxicity Risk Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/aluminum-toxicity-risk-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Assess aluminum toxicity risk in acidic soils and calculate lime requirements.

## Description
This MCP server provides expert tools to evaluate aluminum toxicity in acidic soils. It allows AI agents to determine risk levels using `analyze_aluminum_risk`, identify specific crop vulnerabilities with `check_crop_vulnerability`, estimate root damage via `predict_root_impact`, and calculate necessary soil amendments using `calculate_lime_requirement`. It bridges soil chemistry data with crop-specific biological thresholds to provide actionable agricultural insights.


## Available Tools (4)
- **analyze_aluminum_risk**: 
- **calculate_lime_requirement**: calculate_lime_requirement
- **check_crop_vulnerability**: check_crop_vulnerability
- **predict_root_impact**: predict_root_impact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aluminum Toxicity Risk Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the aluminum toxicity risk for a soil with pH 4.5, exchangeable Al of 2.0 cmolc/kg, and CEC of 10 cmolc/kg for crop 'soybean'?"

**🤖 AI Agent:**
> The aluminum toxicity risk is High, with an Al saturation of 20% and an Al activity that suggests imminent root damage for soybeans.

---

**👤 You:**
> "How much lime do I need for a soil with pH 5.0 and CEC 12 to reach a target pH of 6.0 for corn?"

**🤖 AI Agent:**
> The recommended lime rate is 3.5 tons per hectare to reach the target pH of 6.0.

---

**👤 You:**
> "What is the critical pH for wheat?"

**🤖 AI Agent:**
> The critical pH for wheat is 5.2.


## ❓ FAQ

**Q: How do I know if my soil has aluminum toxicity?**
You can use the `analyze_aluminum_risk` tool by providing the soil pH, exchangeable aluminum, and CEC to determine the risk level.

**Q: Can this tool help with soil remediation?**
Yes, the `calculate_lime_requirement` tool provides specific recommendations for lime application to neutralize aluminum toxicity.

**Q: Does it support different types of crops?**
Yes, the system uses a crop tolerance catalog to assess vulnerability and impact for specific crop IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/aluminum-toxicity-risk-assessment](https://vinkius.com/ai-agent-connect/aluminum-toxicity-risk-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aluminum Toxicity Risk Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aluminum-toxicity-risk-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aluminum Toxicity Risk Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aluminum-toxicity-risk-assessment": {
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
