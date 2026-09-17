# Weight Increment Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/weight-increment-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates optimal weight increases for progressive overload.

## Description
This MCP server provides precise tools for strength training progression. It helps lifters determine the ideal weight increase based on their experience level and exercise type. Use `get_recommended_increment` to find the best next step, `validate_plate_combination` to check if your equipment allows for a specific jump, `get_microloading_strategy` for small-scale increments, and `calculate_progression_percentage` to track intensity shifts.


## Available Tools (4)
- **get_recommended_increment**: Determines the ideal weight increase for the next training session
- **validate_plate_combination**: Checks if a specific weight increase can be physically achieved with the available equipment
- **calculate_progression_percentage**: Calculates how much the weight is increasing relative to the current load
- **get_microloading_strategy**: Provides specific small-scale increment options when standard increments are too large


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weight Increment Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am a beginner male lifting 60kg for a squat. What should my next weight be?"

**🤖 AI Agent:**
> Based on your profile, a recommended increase is 5kg, making your next session 65kg.

---

**👤 You:**
> "I want to add 2.5kg to my current 40kg bicep curl. I have plates of 20, 10, 5, 2.5, and 1.25kg. Is this possible with a 20kg bar?"

**🤖 AI Agent:**
> Yes, it is possible. You will need to add one 1.25kg plate to each side of the bar.

---

**👤 You:**
> "I am an advanced lifter currently at 100kg. What are my microloading options?"

**🤖 AI Agent:**
> For your level, you can use a small increment of 0.5kg or a micro increment of 0.25kg.


## ❓ FAQ

**Q: How does the calculator determine the weight increase?**
The `get_recommended_increment` tool calculates the increase by analyzing your experience level, gender, and whether the exercise is a compound or isolation movement.

**Q: Can I check if I have the right plates for a weight jump?**
Yes, use the `validate_plate_combination` tool. You provide your current weight, the target increment, your available plates, and the bar weight to see if the jump is physically possible.

**Q: What is microloading?**
Microloading is the use of very small weight increments to continue progressing when standard jumps are too large. You can find these options using `get_microloading_strategy`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/weight-increment-calculator](https://vinkius.com/en/ai-agent-connect/weight-increment-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weight Increment Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weight-increment-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weight Increment Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weight-increment-calculator": {
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
