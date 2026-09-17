# Weak Point Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weak-point-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Biomechanical analysis to identify and fix sticking points in compound lifts.

## Description
This MCP server provides deep biomechanical insights into resistance training. By analyzing lift types, sticking point locations, and user anthropometrics, it identifies the primary limiting muscle group. Users can then use `recommend_accessory_work` to find targeted exercises, `generate_technique_cues` for movement optimization, and `get_progression_plan` to build a structured training path to overcome failure points.


## Available Tools (4)
- **get_limiting_factor**: Identifies the primary physiological reason for the lift failure
- **get_progression_plan**: Defines a structured method to overcome the weak point over time
- **recommend_accessory_work**: Provides a curated list of exercises to strengthen the identified weak point
- **generate_technique_cues**: Provides actionable instructions to optimize movement during the lift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weak Point Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm failing my back squat at the bottom. My femur is long. What is happening?"

**🤖 AI Agent:**
> Your long femur creates a significant mechanical disadvantage at the bottom of the squat, placing high torque demands on your quadriceps.

---

**👤 You:**
> "What exercises should I do to fix my bench press lockout?"

**🤖 AI Agent:**
> To improve your bench press lockout, you should focus on triceps-dominant movements like Close-Grip Bench Press and Floor Presses.

---

**👤 You:**
> "Give me a plan to improve my deadlift if my max is 200kg."

**🤖 AI Agent:**
> Based on your 200kg max, your plan includes a 4-week hypertrophy phase followed by a 4-week strength phase, incorporating Romanian Deadlifts and Rack Pulls.


## ❓ FAQ

**Q: How does the analysis determine my weak point?**
The system uses `get_limiting_factor` to correlate your limb lengths and the specific phase of the lift to identify if the failure is due to mechanical leverage or muscle strength.

**Q: Can I get specific exercises for my weakness?**
Yes, once the limiting muscle group is identified, you can use `recommend_accessory_work` to receive a curated list of exercises tailored to your needs.

**Q: Does this help with long-term progress?**
Absolutely. You can use `get_progression_plan` to generate a structured method for increasing load and volume based on your current maximum.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weak-point-analysis](https://vinkius.com/en/ai-agent-connect/weak-point-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weak Point Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weak-point-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weak Point Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weak-point-analysis": {
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
