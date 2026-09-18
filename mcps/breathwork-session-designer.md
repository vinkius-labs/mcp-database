# Breathwork Session Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/breathwork-session-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates structured breathwork protocols tailored to specific techniques and experience levels.

## Description
This MCP server provides a specialized engine for designing personalized breathing exercises. By using tools like `design_session` and `validate_technique_safety`, users can receive structured protocols including breath patterns, hold times, and necessary integration periods. It supports various methodologies such as Wim Hof, Holotropic, Box Breathing, and 4-7-8, adjusting intensity based on whether the user is a beginner, intermediate, or advanced practitioner.


## Available Tools (4)
- **calculate_cycle_metrics**: Determines the rhythmic timing for a single round of a specific technique
- **compare_session_plans**: Allows a user to see how different techniques might fit into their available time
- **design_session**: Generates a complete, structured breathwork protocol based on user requirements
- **validate_technique_safety**: Checks if a specific technique is appropriate for a user's experience level and goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breathwork Session Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a 10-minute Wim Hof session for a beginner looking for energy."

**🤖 AI Agent:**
> Your Wim Hof session is ready: 3 rounds of rapid breathing followed by 30-second breath holds, with a 2-minute integration period at the end.

---

**👤 You:**
> "Is Box Breathing safe for an advanced user?"

**🤖 AI Agent:**
> Yes, Box Breathing is safe and highly effective for advanced users to maintain focus and calm.

---

**👤 You:**
> "What are the timings for a 4-7-8 breathing cycle?"

**🤖 AI Agent:**
> The 4-7-8 pattern consists of a 4-second inhalation, a 7-second breath hold, and an 8-second exhalation.


## ❓ FAQ

**Q: How do I know if a technique is safe for me?**
You can use the `validate_technique_safety` tool to check if a specific technique is appropriate for your current experience level and goals.

**Q: Can I compare different breathing methods?**
Yes, the `compare_session_plans` tool allows you to see how different techniques fit into your available time.

**Q: What kind of protocols are generated?**
The `design_session` tool generates a complete protocol including breath patterns, hold durations, number of rounds, and a mandatory integration period.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/breathwork-session-designer](https://vinkius.com/en/ai-agent-connect/breathwork-session-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breathwork Session Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breathwork-session-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breathwork Session Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breathwork-session-designer": {
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
