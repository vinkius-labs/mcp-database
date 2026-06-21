# Ideal Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ideal-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate your target weight range using scientific formulas like Lorentz, Devine, and Robinson.

## Description
This MCP server provides a precise engine for calculating healthy weight ranges. By utilizing established physiological models including the Lorentz, Devine, and Robinson formulas, alongside a BMI 22 benchmark, it helps you understand your target body mass. Use `calculate_ideal_weight_metrics` to find your range, `assess_bmi_status` to check your current BMI category, and `calculate_weight_gap` to determine exactly how much weight you need to gain or lose to reach your ideal window.


## Available Tools
- **assess_bmi_status**: Assess current BMI and category
- **calculate_ideal_weight_metrics**: Calculate target weight values using various scientific formulas
- **calculate_weight_gap**: Analyze the gap between current weight and target range


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ideal Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my ideal weight range if I am a 180cm male?"

**🤖 AI Agent:**
> Based on the Lorentz, Devine, and Robinson models, your target weight range is approximately 67.5kg to 78.2kg.

---

**👤 You:**
> "I am 165cm and weigh 70kg. What is my BMI?"

**🤖 AI Agent:**
> Your current Body Mass Index (BMI) is 25.7, which falls into the Overweight category.

---

**👤 You:**
> "How much weight do I need to lose to reach a target range of 60kg to 65kg if I currently weigh 72kg?"

**🤖 AI Agent:**
> You are currently 7kg above your maximum target weight and 12kg above your minimum target weight.


## ❓ FAQ

**Q: How accurate are these weight calculations?**
The server uses scientifically recognized models like Devine and Robinson to provide estimates. While highly precise for physiological trends, they should be used as a guide rather than medical advice.

**Q: Can I check my current BMI status?**
Yes, you can use the `assess_bmi_status` tool by providing your height and weight to see your current BMI value and clinical category.

**Q: How do I know how much weight to lose?**
First, find your target range using `calculate_ideal_weight_metrics`. Then, use the `calculate_weight_gap` tool with your current weight and those targets to see the exact difference.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ideal-weight-calculator](https://vinkius.com/mcp/ideal-weight-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ideal Weight Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ideal-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ideal Weight Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ideal-weight-calculator": {
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
