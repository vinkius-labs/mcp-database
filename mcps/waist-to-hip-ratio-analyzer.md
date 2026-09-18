# Waist-to-Hip Ratio Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/waist-to-hip-ratio-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess body fat distribution and health risks using waist-to-hip ratio analysis.

## Description
This MCP server provides specialized tools to analyze body fat distribution through the Waist-to-Hip Ratio (WHR). By comparing waist and hip circumferences, the server can `calculate_whr` to provide the exact ratio, `classify_body_shape` to identify physical profiles like Apple or Pear, `evaluate_health_risk` to determine potential health implications, and `get_fat_distribution_summary` to categorize fat patterns as Android or Gynoid. It uses gender-specific medical thresholds to ensure accurate health risk assessments.


## Available Tools (4)
- **calculate_whr**: Calculate WHR
- **classify_body_shape**: Classify shape
- **evaluate_health_risk**: Evaluate risk
- **get_fat_distribution_summary**: Get summary


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Waist-to-Hip Ratio Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my WHR with a waist of 80cm and hips of 100cm for a female."

**🤖 AI Agent:**
> Your waist-to-hip ratio is 0.80.

---

**👤 You:**
> "What is my body shape if my waist is 95cm and hips are 90cm for a male?"

**🤖 AI Agent:**
> Your body shape is classified as Apple.

---

**👤 You:**
> "Evaluate my health risk with a waist of 105cm and hips of 110cm for a male."

**🤖 AI Agent:**
> Your health risk level is Moderate.


## ❓ FAQ

**Q: How accurate is the health risk assessment?**
The risk assessment is based on established medical thresholds for waist-to-hip ratios, which vary by gender to provide clinically relevant insights.

**Q: What is the difference between Android and Gynoid distribution?**
Android distribution refers to fat concentrated in the abdominal area (apple shape), while Gynoid distribution refers to fat concentrated in the hips and thighs (pear shape).

**Q: Can I use this for both men and women?**
Yes, the tools use gender-specific thresholds to ensure that calculations and risk evaluations are appropriate for both males and females.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/waist-to-hip-ratio-analyzer](https://vinkius.com/en/ai-agent-connect/waist-to-hip-ratio-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Waist-to-Hip Ratio Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `waist-to-hip-ratio-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Waist-to-Hip Ratio Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "waist-to-hip-ratio-analyzer": {
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
