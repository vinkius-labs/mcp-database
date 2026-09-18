# Diabetes Risk Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/diabetes-risk-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess Type 2 Diabetes risk using clinical scoring models.

## Description
This MCP server provides tools to evaluate the probability of developing Type 2 Diabetes. Users can use `calculate_risk_score` to determine their numerical risk and category, `analyze_modifiable_factors` to identify lifestyle areas for improvement, and `generate_prevention_plan` to receive tailored health recommendations based on their specific profile.


## Available Tools (4)
- **analyze_modifiable_factors**: Identify specific aspects of the user's profile that could be improved through lifestyle changes
- **calculate_risk_score**: Compute the numerical risk score and determine the qualitative risk category
- **generate_prevention_plan**: Provide tailored health recommendations based on risk and modifiable factors
- **get_risk_thresholds**: Retrieve the score boundaries used to define risk categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diabetes Risk Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my diabetes risk score if I am 45 years old, have a BMI of 28, a waist circumference of 102cm, am sedentary, have no family history, a blood pressure of 130, and glucose values of [105, 110]?"

**🤖 AI Agent:**
> Your calculated risk score is 12, which places you in the Moderate risk category.

---

**👤 You:**
> "Identify my modifiable risk factors for a 50-year-old with a BMI of 32 and a waist circumference of 110cm who is sedentary."

**🤖 AI Agent:**
> The modifiable factors identified are high BMI and low activity level.

---

**👤 You:**
> "Give me a prevention plan for a high risk score of 18 with factors like high BMI and sedentary lifestyle."

**🤖 AI Agent:**
> To reduce your risk, focus on increasing daily physical activity and implementing a nutritional plan to lower your BMI.


## ❓ FAQ

**Q: How is the risk score calculated?**
The score is calculated using clinical parameters including age, BMI, waist circumference, activity level, family history, blood pressure, and glucose values via the `calculate_risk_score` tool.

**Q: Can I get personalized health advice?**
Yes, by using the `generate_prevention_plan` tool, you can receive specific recommendations tailored to your risk score and modifiable factors.

**Q: What factors can I change to lower my risk?**
You can use `analyze_modifiable_factors` to identify specific areas like activity level or BMI that can be improved through lifestyle changes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/diabetes-risk-assessment](https://vinkius.com/en/ai-agent-connect/diabetes-risk-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Diabetes Risk Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `diabetes-risk-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Diabetes Risk Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "diabetes-risk-assessment": {
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
