# Agent Persona Consistency Scanner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/agent-persona-consistency-scanner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

A precision utility for measuring how closely an LLM adheres to a target persona.

## Description
This MCP server provides advanced linguistic auditing tools to ensure AI agents maintain their intended character. By analyzing text through `analyze_text_consistency`, you can calculate a persona drift score based on pronoun ratios, formality levels, and vocabulary boundaries. Use `get_persona_lexicon` to retrieve specific constraints and `calculate_formality_index` to isolate tone deviations. It is an essential bridge for developers building consistent AI identities.


## Available Tools (3)
- **analyze_text_consistency**: Performs a comprehensive linguistic audit of a text segment to determine how well it fits a specific persona profile
- **calculate_formality_index**: Isolates the formality component to determine if the text's tone is too casual or too formal for the persona
- **get_persona_lexicon**: Retrieves the specific list of forbidden words and required linguistic markers for a given persona


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Persona Consistency Scanner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text for persona consistency: 'I am a professional assistant. I will help you with your tasks.' using persona ID 'prof_01'."

**🤖 AI Agent:**
> { "pronounRatio": 1.0, "formalityScore": 0.0, "violationCount": 0, "driftScore": 0.0 }

---

**👤 You:**
> "What are the forbidden words for the 'Victorian Gentleman' persona?"

**🤖 AI Agent:**
> The forbidden words for the Victorian Gentleman persona include: 'algorithm', 'internet', 'smartphone', and 'digital'.

---

**👤 You:**
> "Check the formality of this text: 'Hey, what's up? I'm just chilling.'"

**🤖 AI Agent:**
> { "contractionDensity": 2.0 }


## ❓ FAQ

**Q: How is the persona drift score calculated?**
The drift score is an aggregate metric derived from deviations in pronoun usage, contraction density (formality), and the presence of forbidden words found via `analyze_text_consistency`.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.

**Q: What is a vocabulary boundary violation?**
A violation occurs when the text contains words defined in the persona's forbidden lexicon, which can be retrieved using `get_persona_lexicon`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/agent-persona-consistency-scanner](https://vinkius.com/ai-agent-connect/agent-persona-consistency-scanner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agent Persona Consistency Scanner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agent-persona-consistency-scanner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agent Persona Consistency Scanner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agent-persona-consistency-scanner": {
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
