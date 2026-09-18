# Waist-to-Height Ratio (WHtR) Health Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/waist-to-height-ratio-whtr-health-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess abdominal obesity and metabolic health risk using waist-to-height ratio.

## Description
This MCP server provides specialized tools to evaluate metabolic health through the Waist-to-Height Ratio (WHtR). Unlike BMI, which only measures total mass, WHtR targets visceral fat to provide a more accurate picture of health risks. You can use `get_whtr_assessment` for a complete health profile, `get_risk_thresholds` to see specific boundaries, `get_ideal_waist_for_height` to find your target waist circumference, or `compare_to_bmi_profile` to understand the difference between your mass-based and metabolic risk.


## Available Tools (4)
- **get_ideal_waist_for_height**: Determines the target waist circumference for a specific height to maintain optimal health
- **get_risk_thresholds**: Informs the user of the specific ratio boundaries used for their assessment
- **get_whtr_assessment**: Provides a complete health assessment based on a user's physical measurements
- **compare_to_bmi_profile**: Explains the qualitative difference between a user's WHtR profile and what a BMI measurement would suggest


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waist-to-Height Ratio (WHtR) Health Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my health risk if my waist is 90cm and my height is 175cm?"

**🤖 AI Agent:**
> Your waist-to-height ratio is 0.51, which places you in the Increased Risk category.

---

**👤 You:**
> "What is the ideal waist circumference for someone 180cm tall?"

**🤖 AI Agent:**
> For a height of 180cm, your target waist circumference should be approximately 82cm to stay within the healthy range.

---

**👤 You:**
> "Compare my WHtR risk to my BMI. My waist is 85cm, height is 170cm, and weight is 70kg."

**🤖 AI Agent:**
> Your BMI is 24.2 (Normal), but your WHtR is 0.50, indicating you are at the upper limit of the healthy range.


## ❓ FAQ

**Q: What is the benefit of WHtR over BMI?**
WHtR is often a better predictor of metabolic risk because it specifically measures abdominal fat, whereas BMI can be influenced by muscle mass.

**Q: How do I use the assessment tool?**
Provide your waist circumference and height in centimeters using the `get_whtr_assessment` tool to receive a full health profile.

**Q: Does ethnicity affect the results?**
Yes, metabolic risk thresholds vary by ethnicity. You can specify your ethnic group in tools like `get_risk_thresholds` for more accurate results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/waist-to-height-ratio-whtr-health-assessment](https://vinkius.com/en/ai-agent-connect/waist-to-height-ratio-whtr-health-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waist-to-Height Ratio (WHtR) Health Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waist-to-height-ratio-whtr-health-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waist-to-Height Ratio (WHtR) Health Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waist-to-height-ratio-whtr-health-assessment": {
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
