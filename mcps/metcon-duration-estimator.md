# MetCon Duration Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/metcon-duration-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Predict workout duration, time caps, and scaling options for metabolic conditioning.

## Description
This MCP server provides specialized tools for metabolic conditioning (MetCon) planning. It helps athletes and coaches predict how long a workout will take using `get_workout_duration`, suggest appropriate time limits with `recommend_time_cap`, and provide tailored movement adjustments via `get_scaling_options`. It also evaluates metabolic demand through `classify_workout_intensity` to ensure workouts match the intended stimulus.


## Available Tools (4)
- **get_scaling_options**: Provides alternative versions of the workout to match an athlete's specific capabilities
- **classify_workout_intensity**: Evaluates the metabolic demand of a workout configuration
- **get_workout_duration**: Predicts how long a specific workout will take to complete
- **recommend_time_cap**: Suggests a maximum time limit to keep the workout within its intended metabolic stimulus


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MetCon Duration Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will a workout of 5 rounds of 10 air squats and 10 push-ups take for an intermediate athlete with low complexity?"

**🤖 AI Agent:**
> The estimated duration for this workout is 320 seconds.

---

**👤 You:**
> "Suggest a time cap for a workout that is expected to take 450 seconds with high intensity."

**🤖 AI Agent:**
> The recommended time cap is 480 seconds.

---

**👤 You:**
> "Give me scaling options for a novice athlete performing snatch movements with high complexity."

**🤖 AI Agent:**
> Suggested scaling: replace snatch with dumbbell cleans and reduce reps to 5 rounds of 5 reps.


## ❓ FAQ

**Q: How accurate are the duration estimates?**
Estimates are calculated by combining movement execution time with transition buffers based on the provided athlete level and movement complexity.

**Q: Can I adjust a workout if it is too difficult?**
Yes, you can use `get_scaling_options` to receive alternative movements and rep schemes tailored to your proficiency level.

**Q: What is a time cap?**
A time cap is a recommended maximum duration to ensure the workout stays within the intended metabolic window.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/metcon-duration-estimator](https://vinkius.com/en/ai-agent-connect/metcon-duration-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MetCon Duration Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metcon-duration-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MetCon Duration Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metcon-duration-estimator": {
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
