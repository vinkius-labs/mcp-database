# Agent Description & Tool Alignment Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agent-description-tool-alignment-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validates alignment between agent descriptions and assigned tools to prevent multi-agent framework errors.

## Description
This MCP server provides critical validation for multi-agent frameworks like CrewAI and AutoGen. It identifies mismatches where an agent's description claims capabilities that its assigned tools cannot perform, or where tools are provided that have no relevance to the agent's persona. By using `tool_analyze_agent_alignment`, the system computes an exact overlap ratio between agent action keywords and tool capability keywords. It also provides `tool_extract_semantic_keywords` for deep text parsing and `tool_get_summary` for high-level health reports on agent functional readiness.


## Available Tools (3)
- **analyze_agent_alignment**: Determines how well an agent's stated purpose matches the tools actually assigned to it
- **extract_keywords**: Isolates the functional core of a text block by identifying relevant action and capability tokens
- **get_summary**: Provides a high-level status report of the agent's functional readiness


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Description & Tool Alignment Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if my agent is ready for its tasks."

**🤖 AI Agent:**
> The agent is Healthy with an alignment score of 0.85 and no misaligned tools detected.

---

**👤 You:**
> "Analyze the alignment for an agent that describes itself as a researcher but only has a calculator tool."

**🤖 AI Agent:**
> Critical: The agent is misaligned. The description implies research capabilities, but the assigned tools have zero overlap with those actions.

---

**👤 You:**
> "Extract the main keywords from this agent description."

**🤖 AI Agent:**
> The extracted keywords are: researcher, data, analysis, report, and collection.


## ❓ FAQ

**Q: What does this tool help prevent?**
It prevents errors in multi-agent frameworks where an agent is assigned tasks it cannot actually perform due to missing or irrelevant tools.

**Q: How is the alignment score calculated?**
The score is the ratio of shared semantic keywords between the agent's description and the tool's functional capabilities.

**Q: Can I use this with CrewAI?**
Yes, it is specifically designed to resolve mismatch errors in frameworks like CrewAI and AutoGen.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agent-description-tool-alignment-checker](https://vinkius.com/mcp/agent-description-tool-alignment-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Description & Tool Alignment Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-description-tool-alignment-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Description & Tool Alignment Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-description-tool-alignment-checker": {
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
