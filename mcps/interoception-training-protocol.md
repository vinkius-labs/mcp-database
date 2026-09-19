# Interoception Training Protocol MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/interoception-training-protocol)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Personalized training plans to improve body awareness and physiological regulation.

## Description
This MCP server provides a specialized system for developing personalized interoception training protocols. By connecting AI agents to physiological awareness frameworks, users can generate structured plans using `generate_protocol` based on their current awareness levels and goals. The system also includes tools like `evaluate_progression_readiness` to track advancement, `suggest_daily_integration_exercise` for real-world application, and `calculate_training_load` to ensure safe and effective practice intensity.


## Available Tools (4)
- **calculate_training_load**: Estimates the cognitive and physiological effort required for a planned session
- **evaluate_progression_readiness**: Determines if a user is ready to move to a more advanced training tier
- **generate_protocol**: Generates a personalized interoception training plan
- **suggest_daily_integration_exercise**: Provides a specific, low-effort exercise to help apply interoceptive skills to daily life


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Interoception Training Protocol** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a training protocol for someone with low awareness who wants to focus on stress regulation, practicing 3 times a week."

**🤖 AI Agent:**
> Your personalized protocol is 'Foundational Somatic Scanning'. It includes 3 sessions per week focusing on broad body scans to build baseline awareness.

---

**👤 You:**
> "I am currently doing Passive Awareness. Suggest an exercise I can do during work."

**🤖 AI Agent:**
> Try the 'Micro-Respiration Check': take 30 seconds to notice the sensation of air entering your nostrils while you type.

---

**👤 You:**
> "Am I ready for Tier 2? My current level is Tier 1, my consistency is 0.9, and my accuracy is 0.85."

**🤖 AI Agent:**
> Yes, you are ready to move to Tier 2 training.


## ❓ FAQ

**Q: How do I start a training plan?**
You can use the `generate_protocol` tool by providing your current awareness level, your primary goal, and how many times per week you wish to practice.

**Q: Can I move to more advanced exercises?**
Yes, you can use `evaluate_progression_readiness` to check if your consistency and accuracy scores meet the requirements for a higher training tier.

**Q: How do I prevent over-training?**
Use the `calculate_training_load` tool to estimate the cognitive and physiological effort of your planned session to ensure it stays within safe limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/interoception-training-protocol](https://vinkius.com/en/ai-agent-connect/interoception-training-protocol)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Interoception Training Protocol** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `interoception-training-protocol` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Interoception Training Protocol** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "interoception-training-protocol": {
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
