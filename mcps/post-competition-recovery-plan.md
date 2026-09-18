# Post-Competition Recovery Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/post-competition-recovery-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Personalized physiological and psychological recovery protocols for athletes.

## Description
This MCP server provides specialized recovery protocols to optimize an athlete's restoration after competition. It uses physiological strain and duration to calculate immediate actions, a 48-hour structured plan, and safe training return timelines. It also includes psychological recovery strategies to manage the mental impact of competition outcomes. Use `get_immediate_actions` for acute stabilization, `get_short_term_plan` for the first two days, `get_training_return_timeline` to plan future training, and `get_psychological_recovery_protocol` for mental health support.


## Available Tools (4)
- **get_immediate_actions**: Provides the first set of recovery interventions to perform immediately after the event concludes
- **get_psychological_recovery_protocol**: Provides mental health and cognitive recovery strategies to manage the post-competition emotional state
- **get_short_term_plan**: Generates a structured schedule for the first 48 hours post-competition
- **get_training_return_timeline**: Determines when the athlete can safely return to various training intensities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Post-Competition Recovery Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just finished a high-intensity race that lasted 120 minutes and I have to fly home tonight. What should I do right now?"

**🤖 AI Agent:**
> Focus on immediate rehydration with electrolytes and gentle mobility exercises to counteract travel stiffness. Prioritize glucose replenishment to restore glycogen stores.

---

**👤 You:**
> "I had a moderate intensity competition for 45 minutes. When can I start training hard again?"

**🤖 AI Agent:**
> You can safely resume high-intensity training in 3 days.

---

**👤 You:**
> "I lost a very intense competition and I'm feeling mentally drained. Help me recover."

**🤖 AI Agent:**
> Focus on cognitive reframing and emotional processing to manage the post-event comedown. Avoid immediate performance reviews and prioritize mental rest.


## ❓ FAQ

**Q: How does the recovery plan account for travel?**
The server includes travel requirements in its calculations, adjusting hydration, mobility, and sleep hygiene protocols to mitigate the impact of travel-induced stress.

**Q: Can I use this to plan my return to training?**
Yes, by using `get_training_return_timeline`, you can determine exactly when it is safe to resume light or high-intensity training based on your competition load.

**Q: What happens if I lost my competition?**
The `get_psychological_recovery_protocol` tool adjusts its recommendations based on the outcome, prioritizing cognitive reframing if the result was a loss.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/post-competition-recovery-plan](https://vinkius.com/en/ai-agent-connect/post-competition-recovery-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Post-Competition Recovery Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `post-competition-recovery-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Post-Competition Recovery Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "post-competition-recovery-plan": {
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
