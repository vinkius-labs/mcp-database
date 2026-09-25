# Novel Development Decision Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/novel-development-decision-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A strategic decision-support engine for authors to synthesize manuscript data and feedback into actionable roadmaps.

## Description
This MCP server provides a suite of strategic tools designed to help authors navigate the complex decision-making process of novel development. By synthesizing manuscript premises, intended readership, and creative constraints, the server helps maintain narrative integrity throughout the drafting process. Authors can use `generate_development_roadmap` to establish high-level strategic directions, `create_chapter_change_brief` for granular revision instructions, and `plan_feedback_response` to evaluate external critiques against their core priorities. The `log_decision_record` tool ensures that every major creative choice is documented with a clear rationale, while `summarize_next_draft_commitments` compiles all necessary actions into a concrete checklist for the next writing session. It is compatible with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client.


## Available Tools (5)
- **summarize_next_draft_commitments**: Compiles the outputs of the roadmap and change briefs into a checklist for the author's next writing session
- **create_chapter_change_brief**: Provides granular, actionable instructions for revising specific chapters based on the development direction
- **generate_development_roadmap**: Synthesizes all input data into a high-level strategic direction for the next phase of writing
- **log_decision_record**: Captures and stores a permanent record of a creative choice to prevent future regression
- **plan_feedback_response**: Evaluates received feedback against the author's priorities to determine which suggestions to adopt


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Novel Development Decision Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need a strategic direction for my thriller novel about a detective in a futuristic city, focusing on improving pacing."

**🤖 AI Agent:**
> To improve pacing in your futuristic noir thriller, the strategic focus should shift toward increasing the frequency of high-stakes investigative breakthroughs in the first half of the manuscript.

---

**👤 You:**
> "My beta readers said the protagonist's motivation is unclear in Chapter 5. How should I handle this?"

**🤖 AI Agent:**
> You should use `create_chapter_change_brief` for Chapter 5 to explicitly link the protagonist's immediate actions to their core internal conflict established in the premise.

---

**👤 You:**
> "I've decided to make the magic system harder to use. How do I record this?"

**🤖 AI Agent:**
> You can use `log_decision_record` to document that the magic system's limitations were increased to heighten the tension and align with the established creative constraints.


## ❓ FAQ

**Q: How does this help with my revision process?**
The server uses `create_chapter_change_brief` to turn high-level strategic directions into specific, actionable instructions for individual chapters, ensuring your revisions stay aligned with your original vision.

**Q: Can I use this to manage feedback from beta readers?**
Yes. The `plan_feedback_response` tool allows you to evaluate incoming feedback against your established revision priorities to decide which suggestions to adopt or reject.

**Q: How do I ensure I don't contradict my own story rules?**
You can use `log_decision_record` to document the rationale behind major creative choices, linking them directly back to your manuscript's premise and constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/novel-development-decision-plan](https://vinkius.com/en/ai-agent-connect/novel-development-decision-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Novel Development Decision Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `novel-development-decision-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Novel Development Decision Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "novel-development-decision-plan": {
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
