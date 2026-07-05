# Ideal Weight Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ideal-weight-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Determine personalized healthy weight ranges and nutritional transition plans using physiological markers.

## Description
The Ideal Weight Calculator provides precise, science-based weight boundaries by integrating multiple anthropometric formulas including Devine, Robinson, Miller, and Ham/Hamwi. Beyond simple BMI, this tool accounts for skeletal frame size via elbow breadth measurements, muscle mass density, and target body fat percentages. Use `calculate_weight_ranges` to find your optimal bounds, `evaluate_bmi_status` to check specific weight points, or `plan_weight_transition` to calculate a safe daily caloric deficit or surplus for reaching your goal weight within a specified timeframe.


## Available Tools (3)
- **calculate_weight_ranges**: Determines the minimum and maximum healthy weight boundaries
- **plan_weight_transition**: Calculates nutritional adjustment for weight change
- **evaluate_bmi_status**: Assesses the health classification of a specific weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ideal Weight Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my healthy weight range if I am a 30-year-old male, 180cm tall, with a large frame?"

**🤖 AI Agent:**
> Based on your height and large frame size, your recommended healthy weight range is between 78.5 kg and 86.2 kg.

---

**👤 You:**
> "I weigh 90kg at 175cm. What is my BMI status?"

**🤖 AI Agent:**
> Your calculated BMI is 29.4, which falls into the Overweight category.

---

**👤 You:**
> "I want to go from 85kg to 80kg in 6 weeks. How many calories should I cut daily?"

**🤖 AI Agent:**
> To reach 80kg in 6 weeks, you need a daily calorie deficit of approximately 592 calories. This transition is considered safe.


## ❓ FAQ

**Q: How does the calculator determine my ideal weight range?**
The `calculate_weight_ranges` tool uses four primary formulas (Devine, Robinson, Miller, and Hamwi) to establish a baseline, then adjusts that range based on your skeletal frame size, muscle mass factor, and target body fat percentage.

**Q: Can I plan a weight loss journey safely?**
Yes. By using `plan_weight_transition`, the tool calculates the necessary daily calorie adjustment and flags whether your target timeframe is safe, adhering to a limit of 1-2 lbs per week.

**Q: What is the purpose of the elbow breadth measurement?**
The elbow breadth measurement (in mm) allows the `calculate_weight_ranges` tool to determine your skeletal frame size (small, medium, or large), which is a critical factor in adjusting ideal mass calculations.


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
3. Set Type to "SSE" (or "streamable HTTP"), enter `ideal-weight-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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
