# Pregnancy Weight Gain Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pregnancy-weight-gain-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Monitor maternal weight trends against IOM guidelines.

## Description
This MCP server provides clinical-grade monitoring for pregnancy weight gain based on the Institute of Medicine (IOM) standards. It allows users to track BMI categories, calculate expected weight gain by gestational week, and analyze weekly velocity to detect deviations from healthy ranges using tools like `get_bmi_recommendations`, `calculate_gain_deviation`, and `analyze_weekly_velocity`.


## Available Tools (3)
- **analyze_weekly_velocity**: Analyzes recent weight changes to detect rapid fluctuations or stagnation
- **get_bmi_recommendations**: Retrieves standardized IOM weight targets based on pre-pregnancy BMI
- **calculate_gain_deviation**: Compares current weight progress against projected ideal weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pregnancy Weight Gain Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my recommended weight gain targets for a pre-pregnancy BMI of 26.5?"

**🤖 AI Agent:**
> For a BMI of 26.5, you fall into the Overweight category. Your recommended total weight gain range is 15 to 25 pounds.

---

**👤 You:**
> "I am at week 20 and my current weight is 160 lbs. My pre-pregnancy weight was 140 lbs and BMI was 23. How am I doing?"

**🤖 AI Agent:**
> You have gained 20 lbs so far. Based on your Normal weight category, the expected gain at week 20 is approximately 14.5 lbs, meaning you are currently 5.5 lbs above the ideal trajectory.

---

**👤 You:**
> "Check if my recent weight gain is healthy: last week I was 158 lbs and this week I am 160 lbs at week 24."

**🤖 AI Agent:**
> Your weekly velocity is 2.0 lbs per week. This is outside the standard healthy range of 0.5 to 1 lb per week for the second and third trimesters.


## ❓ FAQ

**Q: How does the tool determine weight targets?**
The `get_bmi_recommendations` tool uses your pre-pregnancy BMI to identify your category (Underweight, Normal, Overweight, or Obese) and provides the specific weight gain range recommended by IOM.

**Q: Can I track my weekly rate of gain?**
Yes, the `analyze_weekly_velocity` tool compares your previous and current weight to calculate pounds gained per week and checks if it falls within the healthy 0.5-1 lb/week range.

**Q: What happens if my weight gain is outside the expected range?**
The `calculate_gain_deviation` tool calculates exactly how many pounds you are above or below the projected ideal weight for your current gestational week.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pregnancy-weight-gain-tracker](https://vinkius.com/mcp/pregnancy-weight-gain-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pregnancy Weight Gain Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pregnancy-weight-gain-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pregnancy Weight Gain Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pregnancy-weight-gain-tracker": {
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
