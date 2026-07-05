# Advanced BMI & Anthropometric Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/advanced-bmi-anthropometric-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Precision body composition and physiological metric analyzer for fitness and clinical assessment.

## Description
This MCP server provides advanced anthropometric analysis beyond basic Body Mass Index (BMI). It utilizes specific anatomical measurements to estimate health markers, including body fat percentage using the US Navy method, Waist-to-Hip Ratio (WHR) for metabolic risk assessment, and Fat-Free Mass Index (FFMI) for athletes. The toolset includes `calculate_bmi` for standard classification, `analyze_body_composition` for abdominal health risks, `get_athlete_metrics` for muscle density analysis, and `calculate_frame_target_weight` to determine skeletal frame size and ideal weight ranges based on the elbow breadth method.


## Available Tools (4)
- **get_athlete_metrics**: Calculate FFMI and lean body mass
- **calculate_bmi**: Calculate BMI and weight category
- **analyze_body_composition**: Analyze body fat percentage and WHR
- **calculate_frame_target_weight**: Determine skeletal frame size and target weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Advanced BMI & Anthropometric Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my BMI. I weigh 85kg and am 180cm tall."

**🤖 AI Agent:**
> Your BMI is 26.23, which falls into the Overweight category.

---

**👤 You:**
> "Analyze my body composition: male, neck 40cm, waist 95cm, height 180cm."

**🤖 AI Agent:**
> Your estimated body fat is 21.5%. Your Waist-to-Hip Ratio is 0.91, indicating a moderate risk level for visceral fat accumulation.

---

**👤 You:**
> "What is my FFMI? I am 80kg, 180cm tall, and have 15% body fat."

**🤖 AI Agent:**
> Your Fat-Free Mass Index (FFMI) is 23.64, with a total lean body mass of 68 kg.


## ❓ FAQ

**Q: How accurate is the body fat estimation?**
The `analyze_body_composition` tool uses the US Navy method, which provides a reliable estimate of subcutaneous and visceral fat based on circumference measurements without specialized laboratory equipment.

**Q: Can I use this for athletic training assessment?**
Yes, the `get_athlete_metrics` tool is specifically designed to calculate FFMI (Fat-Free Mass Index) and lean body mass, helping athletes assess muscle density relative to their height.

**Q: What measurements are needed for frame size calculation?**
To use `calculate_frame_target_weight`, you need the elbow breadth in millimeters and the user's height in centimeters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/advanced-bmi-anthropometric-analyzer](https://vinkius.com/mcp/advanced-bmi-anthropometric-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Advanced BMI & Anthropometric Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `advanced-bmi-anthropometric-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Advanced BMI & Anthropometric Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "advanced-bmi-anthropometric-analyzer": {
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
