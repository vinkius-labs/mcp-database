# 5x5 Program Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/5x5-program-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured 5x5 strength training programs based on your current lifts and experience.

## Description
This MCP server provides a specialized engine for creating strength training programs using the 5x5 linear progression methodology. It calculates starting weights, determines weekly progression rates, and manages exercise rotation based on your availability. Use `generate_training_program` to build a full multi-week plan, `calculate_starting_weights` to find safe starting points, `evaluate_progression_failure` to manage deloads, and `get_exercise_rotation` to organize your weekly training split.


## Available Tools (4)
- **calculate_starting_weights**: Determines the initial working weight for the first training session
- **evaluate_progression_failure**: Determines if a trainee should initiate a deload protocol
- **generate_training_program**: Generates a complete, multi-week 5x5 strength training program
- **get_exercise_rotation**: Determines the specific sequence of exercises for a trainee


## 💬 Prompt Examples

Here are some examples of how you can interact with the **5x5 Program Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 5x5 program for a beginner who can train 3 days a week. My current lifts are Squat: 100kg, Bench: 60kg, Deadlift: 120kg."

**🤖 AI Agent:**
> Your 5x5 Beginner Program is ready. You will train 3 days per week with a focus on Squat, Bench Press, and Deadlift. Your starting weights are Squat: 80kg, Bench: 48kg, and Deadlift: 96kg.

---

**👤 You:**
> "I've failed my Squat reps twice in a row. Should I deload?"

**🤖 AI Agent:**
> Yes, based on your recent performance, you should initiate a deload. We recommend reducing your weight by 10% for the next session to allow for recovery.

---

**👤 You:**
> "What are my starting weights for an intermediate lifter with a 100kg Squat and 70kg Bench?"

**🤖 AI Agent:**
> For an intermediate level, your calculated starting weights are Squat: 90kg and Bench: 63kg.


## ❓ FAQ

**Q: How do I start a new program?**
You can use the `generate_training_program` tool by providing your current lifts, experience level, goals, and how many days you can train per week.

**Q: What happens if I fail to complete my reps?**
If you hit a plateau, use the `evaluate_progression_failure` tool to determine if you should initiate a deload protocol to recover.

**Q: Can I customize my weekly schedule?**
Yes, the program adjusts the exercise sequence and frequency based on the number of `availableDays` you provide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/5x5-program-generator](https://vinkius.com/en/ai-agent-connect/5x5-program-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **5x5 Program Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `5x5-program-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **5x5 Program Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "5x5-program-generator": {
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
