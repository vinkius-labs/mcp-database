# Pregnancy Weight Gain Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pregnancy-weight-gain-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Monitor pregnancy weight progression using IOM clinical guidelines.

## Description
This MCP server provides clinical weight monitoring for pregnancy. It uses Institute of Medicine (IOM) standards to calculate healthy weight gain ranges based on pre-pregnancy BMI and pregnancy type. Use `get_weight_gain_guidelines` to find specific targets, `calculate_current_status` to check if you are on track, `get_weekly_target_projection` to plan future gain, and `get_trimester_milestones` to see cumulative goals for each trimester.


## Available Tools (4)
- **calculate_current_status**: Compares current weight against historical weight to assess if the user is on track
- **get_trimester_milestones**: Provides a roadmap of what weight gain should look like at the end of each trimester
- **get_weekly_target_projection**: Predicts the necessary weekly weight gain to reach the ideal end-of-pregnancy weight
- **get_weight_gain_guidelines**: Retrieves specific weight gain targets and rules based on the user's physiological profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pregnancy Weight Gain Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a BMI of 22 and I am expecting one baby. What are my weight gain guidelines?"

**🤖 AI Agent:**
> For a BMI of 22 (Normal Weight) and a singleton pregnancy, the recommended total weight gain is between 25 and 35 pounds.

---

**👤 You:**
> "I am 20 weeks pregnant, my pre-pregnancy weight was 130 lbs, and my current weight is 145 lbs. My pre-pregnancy BMI was 21. Am I on track?"

**🤖 AI Agent:**
> Yes, your current weight gain of 15 lbs is within the ideal range for your BMI and gestational age.

---

**👤 You:**
> "What should my weight gain targets be at the end of the second trimester if I have a BMI of 27 and am expecting twins?"

**🤖 AI Agent:**
> For a BMI of 27 and a multiple pregnancy, the target weight gain at the end of the second trimester is approximately 32 pounds.


## ❓ FAQ

**Q: How are the weight gain targets determined?**
Targets are determined using the Institute of Medicine (IOM) guidelines, which factor in your pre-pregnancy BMI and whether you are expecting a singleton or multiple pregnancy.

**Q: Can I use this for twin pregnancies?**
Yes. By using the `isMultiplePregnancy` parameter in the tools, the tracker adjusts all recommendations to account for the higher weight gain requirements of multiple pregnancies.

**Q: How often should I check my status?**
It is recommended to check your status regularly as you progress through your trimesters to ensure you remain within the healthy weight gain range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pregnancy-weight-gain-tracker](https://vinkius.com/en/ai-agent-connect/pregnancy-weight-gain-tracker)
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

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
