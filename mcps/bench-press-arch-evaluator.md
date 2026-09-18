# Bench Press Arch Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bench-press-arch-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Optimize your powerlifting bench press arch for maximum efficiency and competition legality.

## Description
This MCP server provides specialized tools to analyze and optimize a lifter's bench press arch. By analyzing physical metrics like height and shoulder flexibility, the server helps lifters maximize ROM reduction and stability. Use `get_arch_efficiency` to measure how effectively your arch reduces movement, `validate_competition_legality` to ensure your setup meets federation standards, `optimize_leg_drive_position` to find the best foot placement, and `calculate_optimal_setup` to establish a target profile for your training.


## Available Tools (4)
- **calculate_optimal_setup**: Provides a target profile for a lifter to aim for
- **get_arch_efficiency**: Determines how effectively a lifter is reducing their range of motion through their arch
- **optimize_leg_drive_position**: Suggests the best foot placement to maximize arch stability
- **validate_competition_legality**: Checks if the current setup meets standard powerlifting competition requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bench Press Arch Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How efficient is my bench press arch? I am 180cm tall, my arch height is 10cm, and my shoulder flexibility is 0.8."

**🤖 AI Agent:**
> Your arch efficiency is high, providing a significant reduction in range of motion for your height and flexibility profile.

---

**👤 You:**
> "Is my bench press setup legal? My arch is 12cm, shoulder flexibility is 0.7, and my feet are touching the floor."

**🤖 AI Agent:**
> Yes, your current setup meets standard competition requirements.

---

**👤 You:**
> "What is my target setup? I am 175cm tall with a shoulder flexibility of 0.6."

**🤖 AI Agent:**
> Your target profile includes an arch height of 8.5cm, a ROM reduction of 12%, and a posterior foot placement for optimal leg drive.


## ❓ FAQ

**Q: How can I check if my bench press arch is legal for competition?**
You can use the `validate_competition_legality` tool. It checks your arch height, shoulder flexibility, and whether your feet maintain contact with the floor to ensure you meet standard federation requirements.

**Q: How do I improve my arch efficiency?**
Use `get_arch_efficiency` to evaluate your current performance. You can then use `calculate_optimal_setup` to determine the target arch height and ROM reduction you should aim for based on your specific body metrics.

**Q: Can this tool help with my leg drive?**
Yes. The `optimize_leg_drive_position` tool suggests the best foot placement to maximize stability based on your height, arch height, and shoulder flexibility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bench-press-arch-evaluator](https://vinkius.com/en/ai-agent-connect/bench-press-arch-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bench Press Arch Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bench-press-arch-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bench Press Arch Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bench-press-arch-evaluator": {
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
