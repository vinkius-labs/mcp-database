# Assisted Stretch Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/assisted-stretch-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates structured assisted stretching programs based on client flexibility and goals.

## Description
This MCP server provides a specialized engine for creating safe and effective assisted stretching sessions. It uses `plan_session` to generate complete programs, `analyze_flexibility_constraints` to determine safe intensity boundaries, `get_stretch_library` to browse available movements, and `validate_sequence_safety` to audit stretch sequences for physiological safety. It is designed to help practitioners tailor sessions for pain relief, mobility, or athletic performance.


## Available Tools (4)
- **analyze_flexibility_constraints**: Determines the safety boundaries for a client based on their assessment
- **get_stretch_library**: Provides a list of available stretches categorized by target area
- **plan_session**: Generates a complete, structured assisted stretching session plan
- **validate_sequence_safety**: Audits a proposed stretch sequence to ensure it follows physiological safety principles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Assisted Stretch Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a 30-minute mobility session for a client with limited flexibility and tight hip flexors."

**🤖 AI Agent:**
> The 30-minute mobility session for limited flexibility includes: 5 minutes of general warm-up, 10 minutes of gentle hip flexor stretches at low intensity, and 15 minutes of targeted lower body movements.

---

**👤 You:**
> "What are the safe intensity levels for a hypermobile client?"

**🤖 AI Agent:**
> For hypermobile clients, the recommended maximum intensity is moderate to prevent joint instability.

---

**👤 You:**
> "I need a high-intensity performance session for an athlete with normal flexibility focusing on hamstrings."

**🤖 AI Agent:**
> The performance session for hamstring focus includes high-intensity end-range stretches with controlled hold times to optimize muscle length-tension relationships.


## ❓ FAQ

**Q: How does the planner ensure client safety?**
The server uses `validate_sequence_safety` to audit every proposed sequence against physiological principles, ensuring intensity levels match the client's flexibility profile.

**Q: Can I customize the session duration?**
Yes, when using `plan_session`, you can specify the exact number of minutes for the session, and the engine will ensure all stretches fit within that timeframe.

**Q: What types of goals can I set?**
You can choose between pain relief, mobility, or performance as the primary goal for the session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/assisted-stretch-session-planner](https://vinkius.com/en/ai-agent-connect/assisted-stretch-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Assisted Stretch Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `assisted-stretch-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Assisted Stretch Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "assisted-stretch-session-planner": {
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
