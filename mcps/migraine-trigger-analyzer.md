# Migraine Trigger Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/migraine-trigger-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Identifies statistical correlations between lifestyle triggers and migraine episodes.

## Description
This MCP server connects AI agents to advanced pattern analysis for migraine management. It identifies correlations between lifestyle factors and neurological events, accounting for delayed onset and synergistic effects. Use `get_trigger_correlations` to find statistical relationships, `identify_likely_triggers` to pinpoint probable causes, `analyze_trigger_synergies` to detect combined risks, and `get_avoidance_plan` to receive prioritized lifestyle recommendations.


## Available Tools (4)
- **identify_likely_triggers**: Provides a focused list of the most probable culprits for a user's migraines
- **analyze_trigger_synergies**: Detects patterns where multiple triggers occurring together increase migraine risk
- **get_avoidance_plan**: Generates actionable recommendations to reduce migraine frequency
- **get_trigger_correlations**: Identifies which triggers show the strongest statistical relationship with migraine episodes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Migraine Trigger Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze my migraine patterns and tell me which triggers are most likely."

**🤖 AI Agent:**
> Based on your history, the most probable triggers are dehydration and lack of sleep, which show a high correlation with your recent episodes.

---

**👤 You:**
> "Are there any specific trigger combinations I should watch out for?"

**🤖 AI Agent:**
> Yes, there is a significant synergy detected between high stress levels and caffeine consumption that increases your migraine risk.

---

**👤 You:**
> "Give me an avoidance plan based on my data."

**🤖 AI Agent:**
> Your primary recommendation is to increase daily water intake and maintain a consistent sleep schedule to reduce frequency.


## ❓ FAQ

**Q: How does the tool account for delayed onset?**
The `get_trigger_correlations` tool uses an analysis window to look back at trigger exposures that occurred before the migraine episode, accounting for physiological lag.

**Q: Can I identify combinations of triggers?**
Yes, you can use `analyze_trigger_synergies` to detect when multiple triggers occurring together increase your migraine risk more than they would individually.

**Q: What kind of recommendations does it provide?**
The `get_avoidance_plan` tool provides a prioritized list of actionable lifestyle adjustments based on your specific trigger correlations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/migraine-trigger-analyzer](https://vinkius.com/en/ai-agent-connect/migraine-trigger-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Migraine Trigger Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `migraine-trigger-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Migraine Trigger Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "migraine-trigger-analyzer": {
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
