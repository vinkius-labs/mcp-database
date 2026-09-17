# attempt-selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/attempt-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Strategic competition attempt selection for powerlifters.

## Description
This MCP server provides specialized tools for powerlifters to plan their competition strategy. It calculates optimal opener, second, and third attempts for squat, bench press, and deadlift based on gym maximums, competition experience, and risk tolerance. Use `get_attempt_plan` to generate a full lifting sequence, `analyze_risk_profile` to evaluate strategy aggression, `validate_weight_class_compliance` to ensure strength-to-weight ratios are realistic, and `simulate_attempt_success_probability` to predict the likelihood of successful lifts.


## Available Tools (4)
- **analyze_risk_profile**: Evaluates the relationship between an athlete's current gym lifts and their intended risk strategy
- **get_attempt_plan**: Generates a complete set of three attempts for all three lifts based on the athlete's profile
- **simulate_attempt_success_probability**: Provides a statistical estimate of the likelihood of successfully completing each attempt in a sequence
- **validate_weight_class_compliance**: Checks if the athlete's projected attempts are realistic given their weight class constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **attempt-selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my attempts for a squat max of 200kg, bench max of 120kg, and deadlift max of 240kg. I am an intermediate lifter with moderate risk tolerance."

**🤖 AI Agent:**
> Your squat attempts are 170kg, 190kg, and 200kg. Your bench attempts are 102kg, 114kg, and 120kg. Your deadlift attempts are 204kg, 228kg, and 240kg.

---

**👤 You:**
> "I am a novice lifter with a 150kg squat. What is the probability of me successfully making a 140kg second attempt?"

**🤖 AI Agent:**
> The probability of successfully completing a 140kg second attempt with a 150kg gym max as a novice is 0.75.

---

**👤 You:**
> "Is a 300kg deadlift realistic for a 83kg weight class lifter?"

**🤖 AI Agent:**
> Yes, a 300kg deadlift is within the realistic strength profile for an advanced athlete in the 83kg weight class.


## ❓ FAQ

**Q: How does the tool calculate my attempts?**
The tool uses your gym maximums, experience level, and risk tolerance to calculate a sequence of three attempts that balances the goal of maximizing total weight with the need to successfully complete an opener.

**Q: Can I use this for different experience levels?**
Yes, the `get_attempt_plan` tool specifically accounts for novice, intermediate, and advanced lifters to adjust the safety buffer for each attempt.

**Q: What is the difference between conservative and aggressive risk tolerance?**
A conservative profile prioritizes making all three attempts by choosing lower weights, while an aggressive profile targets higher weights to maximize the total, even if the risk of failure is higher.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/attempt-selector](https://vinkius.com/en/ai-agent-connect/attempt-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **attempt-selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `attempt-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **attempt-selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "attempt-selector": {
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
