# Dawn Phenomenon Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/dawn-phenomenon-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Differentiate between Somogyi Effect and Dawn Phenomenon using overnight glucose data.

## Description
This MCP server helps users identify the physiological cause of morning hyperglycemia. By analyzing blood glucose readings from 3:00 AM and 7:00 AM, the `analyze_overnight_glucose` tool distinguishes between the Somogyi Effect (a rebound from nighttime hypoglycemia) and the Dawn Phenomenon (a natural hormonal rise). You can also use `get_glucose_delta_summary` to calculate exact glucose fluctuations or `validate_threshold_compliance` to check for high-risk patterns like Hypoglycemic Rebound or Hormonal Rise.


## Available Tools (3)
- **analyze_overnight_glucose**: Determines the cause of morning hyperglycemia by comparing early morning and waking glucose levels
- **get_glucose_delta_summary**: Provides a focused calculation of the glucose fluctuation between the two measurement points
- **validate_threshold_compliance**: Checks if a specific set of glucose readings falls into known high or low risk categories for medical review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dawn Phenomenon Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My glucose was 65 mg/dL at 3am and 140 mg/dL at 7am. I took 5 units of insulin overnight. What is happening?"

**🤖 AI Agent:**
> The diagnosed condition is Somogyi Effect. It is recommended to reduce overnight insulin or add a bedtime snack.

---

**👤 You:**
> "My glucose was 110 mg/dL at 3am and 150 mg/dL at 7am. I took 10 units of insulin overnight. What is happening?"

**🤖 AI Agent:**
> The diagnosed condition is Dawn Phenomenon. It is recommended to increase overnight insulin or adjust basal timing.

---

**👤 You:**
> "What was the glucose change if my 3am was 90 and my 7am was 100?"

**🤖 AI Agent:**
> The glucose delta is 10 mg/dL.


## ❓ FAQ

**Q: What is the difference between Somogyi Effect and Dawn Phenomenon?**
The Somogyi Effect is a rebound hyperglycemia caused by low blood sugar during the night, while the Dawn Phenomenon is a natural rise in blood sugar due to morning hormone releases.

**Q: How can I use the `analyze_overnight_glucose` tool?**
Provide your 3:00 AM glucose, 7:00 AM glucose, and overnight insulin dose to receive a diagnosis and recommended action.

**Q: Can this tool help with risk assessment?**
Yes, the `validate_threshold_compliance` tool identifies if your readings indicate a Hypoglycemic Rebound or a Hormonal Rise.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/dawn-phenomenon-detector](https://vinkius.com/ai-agent-connect/dawn-phenomenon-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dawn Phenomenon Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dawn-phenomenon-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dawn Phenomenon Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dawn-phenomenon-detector": {
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
