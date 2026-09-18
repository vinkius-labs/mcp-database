# Heart Rate Recovery Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/heart-rate-recovery-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Assess cardiovascular fitness and mortality risk using heart rate recovery metrics.

## Description
This MCP server provides specialized tools to evaluate cardiovascular health by measuring how quickly your heart rate returns to baseline after exercise. Use `calculate_recovery_metrics` to determine your 1-minute and 2-minute recovery drops. You can then use `assess_fitness_and_risk` to translate those numbers into fitness categories and mortality risk indicators based on your age. The server also includes `validate_exercise_intensity` to ensure your workout was strenuous enough for a valid reading, and `generate_training_recommendations` to receive actionable advice tailored to your recovery profile.


## Available Tools (4)
- **assess_fitness_and_risk**: Interpret recovery numbers into fitness categories and mortality risk levels
- **calculate_recovery_metrics**: Calculate raw heart rate recovery values (1-min and 2-min drops)
- **generate_training_recommendations**: Provide actionable exercise advice based on the user's recovery profile
- **validate_exercise_intensity**: Verify if the peak heart rate reached was sufficient for a meaningful assessment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heart Rate Recovery Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my recovery metrics. My peak HR was 170, my 1-min HR was 145, and my 2-min HR was 135."

**🤖 AI Agent:**
> Your 1-minute recovery is 25 BPM and your 2-minute recovery is 35 BPM.

---

**👤 You:**
> "I am 35 years old. My 1-min recovery was 30 BPM and my 2-min recovery was 45 BPM. What is my fitness level and risk?"

**🤖 AI Agent:**
> Your cardiovascular fitness is categorized as Good, and your mortality risk is Low.

---

**👤 You:**
> "My 1-min recovery was 15 BPM and my fitness category is Poor. What should I do?"

**🤖 AI Agent:**
> Your primary training focus should be building a steady aerobic base. It is recommended to engage in consistent, moderate-intensity aerobic exercise to improve your cardiovascular efficiency.


## ❓ FAQ

**Q: How do I know if my exercise was intense enough?**
You can use the `validate_exercise_intensity` tool. It compares your peak heart rate against your age-predicted maximum to confirm if the session was sufficient for a valid assessment.

**Q: What do the recovery numbers mean?**
The recovery numbers represent the drop in beats per minute (BPM) from your peak heart rate. A larger drop generally indicates better cardiovascular efficiency.

**Q: Can this tool provide training advice?**
Yes. After assessing your fitness, you can use `generate_training_recommendations` to get specific guidance on training focus and intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/heart-rate-recovery-calculator](https://vinkius.com/en/ai-agent-connect/heart-rate-recovery-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heart Rate Recovery Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heart-rate-recovery-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heart Rate Recovery Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heart-rate-recovery-calculator": {
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
