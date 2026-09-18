# BMI Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bmi-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate Body Mass Index and weight health metrics.

## Description
This MCP server provides precise Body Mass Index (BMI) calculations and clinical weight analysis. Use `calculate_bmi` to find your BMI category, `get_healthy_weight_range` to see your target weight spectrum, and `calculate_weight_proximity` to determine how far you are from a healthy weight. It also includes `convert_imperial_to_metric` to easily handle measurements in pounds and feet/inches.


## Available Tools (4)
- **calculate_bmi**: 
- **calculate_weight_proximity**: 
- **convert_imperial_to_metric**: 
- **get_healthy_weight_range**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BMI Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my BMI if I weigh 70kg and am 175cm tall?"

**🤖 AI Agent:**
> Your BMI is 22.86, which falls into the Normal weight category.

---

**👤 You:**
> "I am 180cm tall. What is my healthy weight range?"

**🤖 AI Agent:**
> For a height of 180cm, your healthy weight range is between 60.0kg and 81.0kg.

---

**👤 You:**
> "I weigh 95kg and am 175cm tall. How far am I from my healthy weight range?"

**🤖 AI Agent:**
> You are 14.0kg above your healthy weight range.


## ❓ FAQ

**Q: How do I calculate my BMI?**
You can use the `calculate_bmi` tool by providing your weight in kilograms and height in centimeters.

**Q: Can I use imperial units like pounds and feet?**
Yes, you can use `convert_imperial_to_metric` to transform your weight in lbs and height in feet/inches into metric units for calculation.

**Q: How can I find my healthy weight range?**
Use the `get_healthy_weight_range` tool with your height in centimeters to see the weight bounds for a normal BMI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bmi-calculator](https://vinkius.com/en/ai-agent-connect/bmi-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BMI Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bmi-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BMI Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bmi-calculator": {
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
