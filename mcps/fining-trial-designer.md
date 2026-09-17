# Fining Trial Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fining-trial-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Design precise fining trials to correct wine issues like haze or astringency.

## Description
This MCP server provides specialized tools for winemakers to design safe and effective fining trials. Use `design_fining_trial` to generate comprehensive dose-response plans, `calculate_overfining_threshold` to determine safe dosage limits, and `get_agent_capabilities` to understand the technical profile of agents like Bentonite or PVPP. You can also use `validate_sensory_plan` to ensure your evaluation criteria correctly monitor for both target correction and overfining risks.


## Available Tools (4)
- **calculate_overfining_threshold**: Determines the safe upper limit for a specific agent to prevent loss of wine quality
- **design_fining_trial**: Generates a comprehensive trial plan based on a specific wine issue and available agents
- **get_agent_capabilities**: Retrieves the technical profile and target issues for a specific fining agent
- **validate_sensory_plan**: Ensures that the proposed evaluation criteria are sufficient to detect both the target correction and potential overfining


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fining Trial Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a wine with haze issues and I have Bentonite available. Can you design a trial for me?"

**🤖 AI Agent:**
> I have generated a trial design for haze correction using Bentonite. The trial will cover a dose range from 10 to 50 g/hL with 5 concentration levels, focusing on stability and clarity.

---

**👤 You:**
> "What is the safe dose for Charcoal in a 500L batch of wine?"

**🤖 AI Agent:**
> The safe maximum dose for Charcoal in a 500L volume is 25 g/hL, with a medium risk level for overfining.

---

**👤 You:**
> "What does PVPP target?"

**🤖 AI Agent:**
> PVPP is a synthetic polymer primarily designed to target and remove bitter phenols from wine.


## ❓ FAQ

**Q: How do I prevent overfining my wine?**
You can use the `calculate_overfining_threshold` tool to find the safe maximum dose for a specific agent based on your wine volume.

**Q: Can I design a trial for multiple agents at once?**
Yes, the `design_fining_trial` tool allows you to provide a list of available agents to generate a comparative trial plan.

**Q: How do I know if my sensory evaluation is sufficient?**
Use the `validate_sensory_plan` tool to check if your proposed criteria are adequate to detect both the target correction and potential overfining.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fining-trial-designer](https://vinkius.com/en/ai-agent-connect/fining-trial-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fining Trial Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fining-trial-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fining Trial Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fining-trial-designer": {
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
