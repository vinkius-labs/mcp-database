# Infrared Sauna Dosage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/infrared-sauna-dosage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Personalized infrared sauna protocols based on physiological goals and health status.

## Description
This MCP server provides precise infrared sauna guidance by calculating optimal session parameters. Using tools like `calculate_session_protocol` and `calculate_weekly_schedule`, users can determine the ideal duration, temperature, and frequency for goals such as detox, relaxation, or cardiovascular health. It also includes `estimate_cumulative_benefits` to project long-term physiological impact and `get_safety_guidelines` to ensure safe thermal exposure based on individual health status and experience levels.


## Available Tools (4)
- **calculate_session_protocol**: Determines the specific parameters for a single sauna session based on user profile and intent
- **calculate_weekly_schedule**: Determines how many times per week a user should utilize the sauna to achieve their goal safely
- **estimate_cumulative_benefits**: Projects the physiological advantages of adhering to a specific dosage over time
- **get_safety_guidelines**: Provides specific environmental and behavioral constraints based on the user's health and experience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infrared Sauna Dosage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a beginner looking for relaxation. What is my recommended sauna protocol?"

**🤖 AI Agent:**
> For a beginner seeking relaxation, it is recommended to use the sauna at 50°C for 15 minutes, once or twice a week.

---

**👤 You:**
> "How many sessions per week do I need for detox if I do 20-minute sessions?"

**🤖 AI Agent:**
> To achieve detox goals with 20-minute sessions, you should aim for 3 to 4 sessions per week.

---

**👤 You:**
> "What are the long-term benefits of a cardiovascular sauna protocol?"

**🤖 AI Agent:**
> Consistent adherence to a cardiovascular sauna protocol can lead to improved heart rate variability and enhanced thermal stress adaptation.


## ❓ FAQ

**Q: How do I know if a sauna session is safe for me?**
You can use the `get_safety_guidelines` tool, which provides specific environmental and behavioral constraints based on your health status and experience level.

**Q: Can I plan a weekly routine with this tool?**
Yes, the `calculate_weekly_schedule` tool helps you determine how many times per week you should use the sauna to achieve your specific goals safely.

**Q: What information do I need to provide for a protocol?**
To use `calculate_session_protocol`, you should provide your session goal (detox, relaxation, or cardiovascular), your experience level, and your current health status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/infrared-sauna-dosage-calculator](https://vinkius.com/en/ai-agent-connect/infrared-sauna-dosage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infrared Sauna Dosage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infrared-sauna-dosage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infrared Sauna Dosage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infrared-sauna-dosage-calculator": {
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
