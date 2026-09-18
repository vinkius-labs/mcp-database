# Holistic Breathing Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/holistic-breathing-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Evaluates breathing efficiency and physiological patterns to identify dysfunctions.

## Description
This MCP server provides a comprehensive diagnostic suite for respiratory health. It allows AI agents to assess breathing mechanics, chemical respiratory drive, and overall physiological stability. By using tools like `analyze_breathing_pattern` and `evaluate_co2_tolerance`, agents can determine a user's breathing score, identify specific dysfunction indicators, and establish ranked correction priorities. The server also provides `get_breathing_benchmarks` to compare individual metrics against healthy physiological norms.


## Available Tools (4)
- **analyze_breathing_pattern**: Evaluates the primary mechanics of the user's breath to determine efficiency
- **calculate_breathing_score**: Generates a holistic assessment by synthesizing mechanical and chemical data
- **evaluate_co2_tolerance**: Assesses the user's chemical respiratory drive and CO2 sensitivity
- **get_breathing_benchmarks**: Provides reference ranges for healthy breathing metrics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Holistic Breathing Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my breathing: I take 18 breaths per minute, my depth is 5, and I use my diaphragm."

**🤖 AI Agent:**
> Your breathing pattern is efficient with a high score due to diaphragmatic usage and a stable rate.

---

**👤 You:**
> "How is my CO2 tolerance? I can hold my breath for 30 seconds and I've done 3 successful holds."

**🤖 AI Agent:**
> Your CO2 tolerance is moderate, indicating a stable chemical respiratory drive.

---

**👤 You:**
> "Give me a full breathing assessment based on these results: pattern score 60 and CO2 tolerance level moderate."

**🤖 AI Agent:**
> Your final breathing score is 65. Primary correction priority is mechanical adjustment to improve diaphragmatic engagement.


## ❓ FAQ

**Q: What can this tool assess?**
It assesses breathing rate, depth, diaphragmatic usage, CO2 tolerance, and provides a holistic breathing score.

**Q: How are correction priorities determined?**
Priorities are ranked based on the severity of identified dysfunctions, such as prioritizing mechanical adjustments if breathing patterns are highly inefficient.

**Q: Does it provide age-specific data?**
Yes, by using the `get_breathing_benchmarks` tool with a user's age, the server provides age-specific reference ranges.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/holistic-breathing-assessment](https://vinkius.com/en/ai-agent-connect/holistic-breathing-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Holistic Breathing Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `holistic-breathing-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Holistic Breathing Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "holistic-breathing-assessment": {
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
