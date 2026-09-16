# Surf Injury Prevention Program MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-injury-prevention-program)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Customized injury prevention protocols for surfers based on injury history and biomechanics.

## Description
This MCP server provides specialized tools to help surfers stay in the water longer. By using `analyze_injury_risk`, agents can quantify a surfer's risk profile. The `generate_prevention_program` tool creates personalized exercise protocols by analyzing injury history, surf intensity, and anatomical weaknesses. Additionally, users can access specific movements via `get_exercise_library` and manage their training advancement with `calculate_progression_logic`.


## Available Tools (4)
- **analyze_injury_risk**: Quantify the overall risk profile of a surfer
- **calculate_progression_logic**: Determine how a user should advance their training
- **generate_prevention_program**: Generate a complete, personalized injury prevention protocol
- **get_exercise_library**: Retrieve a filtered list of corrective exercises


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Injury Prevention Program** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have had chronic shoulder pain and I surf at a high intensity. What is my risk profile?"

**🤖 AI Agent:**
> Your risk profile is High, and it is recommended to follow a more conservative training volume to ensure stability.

---

**👤 You:**
> "Generate a prevention program for a beginner surfer with weak core stability and low surf intensity."

**🤖 AI Agent:**
> Your program includes core stability exercises like planks and bird-dogs, to be performed 2 times per week, with a gradual progression in hold duration.

---

**👤 You:**
> "I am an intermediate surfer with a history of knee instability. What exercises can help with stability?"

**🤖 AI Agent:**
> To improve knee stability, you should focus on lateral lunges and single-leg balance exercises.


## ❓ FAQ

**Q: How does the program determine my risk level?**
The `analyze_injury_risk` tool evaluates your past injury history alongside your current surf intensity to categorize your risk level.

**Q: Can I get specific exercises for my shoulder?**
Yes, you can use `get_exercise_library` to find specific exercises for the shoulder, back, knee, core, or hip.

**Q: How often should I perform the recommended exercises?**
The `generate_prevention_program` tool calculates a specific weekly frequency tailored to your surf intensity and injury risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-injury-prevention-program](https://vinkius.com/en/ai-agent-connect/surf-injury-prevention-program)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Injury Prevention Program** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-injury-prevention-program` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Injury Prevention Program** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-injury-prevention-program": {
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
