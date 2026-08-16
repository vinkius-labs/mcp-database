# Conversation Termination Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/conversation-termination-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Prevents runaway agent loops by detecting repetition and stagnation.

## Description
This MCP server provides critical governance tools for multi-agent systems like AutoGen or CrewAI. It prevents 'hallucination spirals' and infinite loops by monitoring conversation health. Using `get_termination_status`, agents can check if they have reached the turn limit or signaled completion. The `analyze_message_repetition` tool detects semantic loops through Jaccard similarity, while `check_progress_plateau` identifies when a conversation has stalled by monitoring changes in subject matter. Connect via Vinkius Edge to give your AI agents the ability to self-regulate and terminate efficiently.


## Available Tools (3)
- **analyze_message_repetition**: Checks for semantic loops by comparing the similarity of recent assistant outputs
- **check_progress_plateau**: Detects if the conversation has stopped moving forward by monitoring subject matter changes
- **get_termination_status**: Determines if the current conversation state warrants an immediate stop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Conversation Termination Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the current conversation should end."

**🤖 AI Agent:**
> The conversation should continue as no termination criteria have been met.

---

**👤 You:**
> "Is the agent repeating itself?"

**🤖 AI Agent:**
> Yes, the similarity score between recent messages is too high, indicating a repetitive loop.

---

**👤 You:**
> "Has the conversation reached the maximum number of turns?"

**🤖 AI Agent:**
> Yes, the turn count has reached the user-defined limit.


## ❓ FAQ

**Q: How does this prevent infinite loops?**
It uses `get_termination_status` to monitor turn counts and `analyze_message_repetition` to detect when agents are repeating the same content, triggering a stop signal.

**Q: Can I define my own completion signals?**
Yes, you can provide a custom list of phrases to `get_termination_status` that will act as termination keywords.

**Q: What is a progress plateau?**
A plateau occurs when the conversation stops progressing. The `check_progress_plateau` tool detects this by checking if new information or subjects are being introduced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/conversation-termination-evaluator](https://vinkius.com/ai-agent-connect/conversation-termination-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Conversation Termination Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `conversation-termination-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Conversation Termination Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "conversation-termination-evaluator": {
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
