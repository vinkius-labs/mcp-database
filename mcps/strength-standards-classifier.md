# Strength Standards Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/strength-standards-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Classifies lifts by strength standards and provides progression targets.

## Description
This MCP server connects AI agents to professional strength standards. It allows users to determine their classification level (Novice, Intermediate, Advanced, or Elite) for various lifts. By using `get_lift_classification`, you can find your current percentile and specific weight targets for your next milestone. You can also use `get_milestone_targets` to plan your training progression and `list_supported_lifts` to see which movements are available for analysis.


## Available Tools (4)
- **list_supported_lifts**: Informs the user of which lifts can be analyzed
- **get_lift_classification**: Determines an individual's current strength level and provides progression targets
- **get_milestone_targets**: Calculates the specific weight required to achieve upcoming strength levels
- **get_strength_percentile**: Provides a statistical context of where a lift sits within a population


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Strength Standards Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just squatted 100kg at a body weight of 80kg. What is my strength level?"

**🤖 AI Agent:**
> Your squat is classified as Intermediate, placing you in the 65th percentile.

---

**👤 You:**
> "What weight do I need to hit to become an Advanced bench presser at 90kg body weight?"

**🤖 AI Agent:**
> To reach the Advanced level for bench press at 90kg, you need to lift 115kg.

---

**👤 You:**
> "List all the lifts I can analyze with this tool."

**🤖 AI Agent:**
> The supported lifts are squat, bench_press, deadlift, and overhead_press.


## ❓ FAQ

**Q: Which lifts are supported?**
You can use `list_supported_lifts` to see the full list of available movements like squat, bench press, and deadlift.

**Q: How do I know my next training goal?**
Use the `get_milestone_targets` tool to calculate the exact weight needed to reach the next strength classification level.

**Q: Does gender affect the classification?**
Yes, strength standards are calculated based on biological gender to ensure accurate and fair classification.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/strength-standards-classifier](https://vinkius.com/en/ai-agent-connect/strength-standards-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Strength Standards Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `strength-standards-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Strength Standards Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "strength-standards-classifier": {
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
