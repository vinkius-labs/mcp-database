# Verb Conjugation Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/verb-conjugation-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Deterministic morphological engine for Romance language verb conjugation.

## Description
This MCP server provides a deterministic morphological engine for generating accurate verb conjugations across Spanish, French, Italian, and Portuguese. It handles complex stem changes, precise accentuation, and strict clitic attachment rules. Use `conjugate_verb` to get specific forms, `get_conjugation_pattern` to identify morphological templates, or `validate_clitic_placement` to ensure correct pronoun positioning.


## Available Tools (3)
- **conjugate_verb**: Provides the primary conjugation of a specific verb based on grammatical parameters
- **get_conjugation_pattern**: Returns the morphological patterns or "templates" for a specific verb
- **validate_clitic_placement**: Checks if a specific combination of verb form and pronoun placement is grammatically valid


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Verb Conjugation Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Conjugate the Spanish verb 'hablar' in the present indicative for the first person singular."

**🤖 AI Agent:**
> hablo

---

**👤 You:**
> "What is the conjugation pattern for the French verb 'manger'?"

**🤖 AI Agent:**
> Regular -er verb pattern.

---

**👤 You:**
> "Conjugate the Portuguese verb 'querer' in the present indicative for the third person singular."

**🤖 AI Agent:**
> quer


## ❓ FAQ

**Q: Which languages are supported?**
The engine supports Spanish, French, Italian, and Portuguese.

**Q: How do I check if a pronoun placement is correct?**
You can use the `validate_clitic_placement` tool to verify if a pronoun should be proclitic or enclitic for a specific verb form and mood.

**Q: Does it handle irregular verbs?**
Yes, the engine identifies highly irregular verbs and stem-changing (weak) verbs, providing the specific rule applied in the response.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/verb-conjugation-engine](https://vinkius.com/ai-agent-connect/verb-conjugation-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Verb Conjugation Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `verb-conjugation-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Verb Conjugation Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "verb-conjugation-engine": {
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
