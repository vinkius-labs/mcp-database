# Strength Standards Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/strength-standards-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Classify weightlifting strength levels and predict future milestones.

## Description
The Strength Standards Checker is a performance analysis tool designed to help lifters track their progression. By using the `check_strength_level` tool, you can determine your current strength tier (from Untrained to Elite) based on your weight lifted, body weight, exercise type, and sex. Additionally, use `calculate_next_milestone` to identify exactly how much more weight you need to lift to reach your next goal, and `get_supported_benchmarks` to see all compatible exercises like Squat, Bench Press, and Deadlift.


## Available Tools (3)
- **get_supported_benchmarks**: Retrieve supported exercises and sexes
- **calculate_next_milestone**: Calculate weight needed for next strength tier
- **check_strength_level**: Check current strength level based on a lift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strength Standards Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just squatted 100kg and I weigh 80kg. What is my strength level for a male?"

**🤖 AI Agent:**
> Your strength level for Squat is Intermediate with a strength ratio of 1.25.

---

**👤 You:**
> "How much weight do I need to bench press to reach the next level if I am currently at Novice level, weighing 75kg, and I am female?"

**🤖 AI Agent:**
> To reach the Intermediate level, you need to lift 42.0 kg. This represents a required ratio increase of 0.05.

---

**👤 You:**
> "What are the valid exercises I can check?"

**🤖 AI Agent:**
> The supported exercises are: Squat, Bench Press, Deadlift, Overhead Press, and Power Clean.


## ❓ FAQ

**Q: How is my strength level calculated?**
The tool calculates your relative strength by dividing the weight lifted by your body weight and compares this ratio against established benchmarks for your specific exercise and sex.

**Q: What exercises are supported?**
Currently, the tool supports Squat, Bench Press, Deadlift, Overhead Press, and Power Clean.

**Q: Can I predict my next strength milestone?**
Yes, by using the `calculate_next_milestone` tool, you can find out the target weight required to reach your next progression tier.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/strength-standards-checker](https://vinkius.com/mcp/strength-standards-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strength Standards Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `strength-standards-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strength Standards Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strength-standards-checker": {
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
