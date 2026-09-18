# Air Quality Health Impact Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/air-quality-health-impact-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess health risks and symptom likelihood from air quality levels.

## Description
This MCP server provides specialized tools to evaluate how air quality affects human health. It calculates risk categories, predicts symptom likelihood, and provides activity recommendations based on AQI, pollutant types, and individual profiles. Use `get_risk_assessment` for a full health profile, `get_symptom_probability` to predict physiological effects, `get_activity_guidelines` for lifestyle adjustments, and `check_sensitive_group_status` to identify high-risk individuals.


## Available Tools (4)
- **check_sensitive_group_status**: Determines if an individual requires heightened monitoring based on their profile
- **get_activity_guidelines**: Recommends specific lifestyle or physical activity changes to mitigate health impact
- **get_risk_assessment**: Provides a comprehensive health risk profile for an individual based on current air conditions
- **get_symptom_probability**: Estimates the likelihood of experiencing specific physiological symptoms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Air Quality Health Impact Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my health risk if the AQI is 150 for Ozone and I am 70 years old with a respiratory condition?"

**🤖 AI Agent:**
> Your health risk category is Unhealthy for Sensitive Groups. You may experience increased respiratory symptoms, and it is recommended to reduce prolonged outdoor exertion.

---

**👤 You:**
> "What symptoms might I expect if I've been exposed to Particulate Matter at an AQI of 50 for 30 minutes?"

**🤖 AI Agent:**
> At an AQI of 50, the probability of experiencing respiratory symptoms is low.

---

**👤 You:**
> "What should I do if the AQI is 200 and I am in a sensitive group?"

**🤖 AI Agent:**
> With an AQI of 200, you should limit outdoor activities, stay indoors in a filtered environment, and avoid vigorous physical exertion.


## ❓ FAQ

**Q: How does this tool determine health risk?**
The `get_risk_assessment` tool calculates risk by combining the Air Quality Index (AQI) value with individual factors like age and pre-existing health conditions.

**Q: Can I get recommendations for physical activities?**
Yes, you can use `get_activity_guidelines` to receive specific recommendations for adjusting your activity levels based on current air quality and your sensitivity status.

**Q: Does it identify sensitive populations?**
Yes, the `check_sensitive_group_status` tool identifies if an individual is at higher risk due to age or existing health conditions relative to specific pollutants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/air-quality-health-impact-assessment](https://vinkius.com/en/ai-agent-connect/air-quality-health-impact-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Air Quality Health Impact Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `air-quality-health-impact-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Air Quality Health Impact Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "air-quality-health-impact-assessment": {
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
