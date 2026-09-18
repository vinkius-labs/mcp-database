# Nervous System Regulation Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nervous-system-regulation-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Personalized regulation strategies based on Polyvagal Theory.

## Description
This MCP server provides tools to help users navigate their autonomic nervous system states using Polyvagal Theory. It can generate customized activity plans with `get_regulation_plan`, describe physiological states using `get_state_characteristics`, verify if symptoms match a reported state via `validate_symptom_alignment`, and log session outcomes with `track_regulation_progress`.


## Available Tools (4)
- **validate_symptom_alignment**: Checks if the reported symptoms are consistent with the reported autonomic state
- **get_regulation_plan**: Generates a customized set of activities to help a user move toward a more regulated state
- **get_state_characteristics**: Provides a description of what a specific autonomic state feels like
- **track_regulation_progress**: Records the outcome of a regulation session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nervous System Regulation Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I feel very anxious and my heart is racing. I have 15 minutes. What should I do?"

**🤖 AI Agent:**
> Since you are experiencing sympathetic activation, I recommend these grounding activities: 5 minutes of deep belly breathing and 10 minutes of gentle stretching.

---

**👤 You:**
> "I feel numb and disconnected. I have 10 minutes."

**🤖 AI Agent:**
> You appear to be in a dorsal state. I suggest 10 minutes of gentle sensory stimulation to help with mobilization.

---

**👤 You:**
> "What does the ventral state feel like?"

**🤖 AI Agent:**
> The ventral state is characterized by feelings of safety, social engagement, and calm presence.


## ❓ FAQ

**Q: What is Polyvagal Theory?**
It is a theory describing how the autonomic nervous system regulates our physiological states, including safety, mobilization, and shutdown.

**Q: How do I know which state I am in?**
You can use the `get_state_characteristics` tool to understand the physical and emotional indicators of ventral, sympathetic, or dorsal states.

**Q: Can I track my progress over time?**
Yes, you can record the effectiveness of your regulation sessions using `track_regulation_progress`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nervous-system-regulation-planner](https://vinkius.com/en/ai-agent-connect/nervous-system-regulation-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nervous System Regulation Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nervous-system-regulation-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nervous System Regulation Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nervous-system-regulation-planner": {
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
