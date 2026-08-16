# Agent Loop Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-loop-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [observability](../categories/observability.md)

Detects cyclic delegation and repetitive conversation loops in multi-agent systems.

## Description
Agent Loop Detector provides specialized monitoring for multi-agent orchestration frameworks like CrewAI, AutoGen, and LangGraph. It identifies infinite loops by creating a deterministic fingerprint for every agent turn (agent_id, action_type, and target_id). When a specific fingerprint repeats beyond a configurable threshold, the system flags the loop, calculates the cycle length, and identifies the trapped agents. Use `check_for_loops` to detect cycles, `get_fingerprint_analysis` to view fingerprint frequency, and `calculate_current_cycle_metrics` to analyze the intensity and purity of a detected loop.


## Available Tools (3)
- **calculate_current_cycle_metrics**: Analyzes a specific detected cycle to provide detailed insights into the nature of the loop
- **check_for_loops**: Determines if the current sequence of agent actions has entered an infinite loop or repetitive cycle
- **get_fingerprint_analysis**: Provides a breakdown of how many times each unique action fingerprint has occurred in the current history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Loop Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my agents are stuck in a loop."

**🤖 AI Agent:**
> loop_detected: true, cycle_length: 3, trapped_agent_ids: ['agent_a', 'agent_b']

---

**👤 You:**
> "How many times has the current action fingerprint occurred?"

**🤖 AI Agent:**
> The fingerprint 'agent_1_call_agent_2' has occurred 4 times.

---

**👤 You:**
> "Analyze the metrics for the detected cycle."

**🤖 AI Agent:**
> is_pure_loop: true, loop_intensity: 0.45


## ❓ FAQ

**Q: How does the loop detection work?**
The system generates a unique fingerprint for each agent action. If the same fingerprint appears multiple times based on your threshold, a loop is flagged.

**Q: What is a deterministic fingerprint?**
It is a unique identifier created by combining the agent ID, the action type, and the target ID of a specific turn.

**Q: Can I adjust the sensitivity of detection?**
Yes, you can use the `maxRepeatThreshold` parameter in the `check_for_loops` tool to define how many repetitions trigger a detection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-loop-detector](https://vinkius.com/ai-agent-connect/agent-loop-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Loop Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-loop-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Loop Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-loop-detector": {
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
