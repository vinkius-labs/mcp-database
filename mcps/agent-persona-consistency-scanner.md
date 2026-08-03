# Agent Persona Consistency Scanner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agent-persona-consistency-scanner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [quality-assurance](../categories/quality-assurance.md)

Verify LLM adherence to defined personas by analyzing pronoun ratios, formality scores, and vocabulary violations.

## Description
The Agent Persona Consistency Scanner MCP server provides a precise engine for auditing LLM outputs against specific persona constraints. It calculates exact pronoun usage ratios (1st person vs 3rd person), determines formality scores by measuring contraction density per 100 words, and identifies vocabulary boundary violations using a custom lexicon of forbidden terms. By utilizing tools like `analyze_pronouns`, `calculate_formality`, `check_vocabulary`, and `scan_persona`, developers can quantify persona drift and ensure consistent agent behavior across different prompts.


## Available Tools (4)
- **check_vocabulary**: Check for forbidden words in the provided text
- **calculate_formality**: Calculate the formality score based on contraction count
- **scan_persona**: Perform a comprehensive persona drift analysis
- **analyze_pronouns**: Analyze the ratio of 1st person to 3rd person pronouns in text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agent Persona Consistency Scanner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this text for persona consistency: 'I am very happy to meet you. He said that the weather is nice.'"

**🤖 AI Agent:**
> The pronoun ratio analysis shows a 50% usage of 1st person pronouns and 50% 3rd person pronouns.

---

**👤 You:**
> "Check if the following text contains any forbidden words: ['bad', 'error'], Text: 'This is a bad error.'"

**🤖 AI Agent:**
> The vocabulary check identified 2 violations: 'bad' and 'error'.

---

**👤 You:**
> "Calculate the formality of: 'Don't you think it's great?'"

**🤖 AI Agent:**
> The formality score is high due to the presence of 2 contractions ('Don't', 'it's') in a short string.


## ❓ FAQ

**Q: How does the formality score calculation work?**
The `calculate_formality` tool counts the number of contractions found in the input text and calculates a density score relative to the total word count (contractions per 100 words).

**Q: Can I use a custom list of forbidden words?**
Yes, the `check_vocabulary` tool accepts a JSON array of strings representing your restricted lexicon to identify any violations in the text.

**Q: What is included in a full persona drift analysis?**
The `scan_persona` tool performs an integrated audit, combining pronoun ratio analysis, formality scoring, and vocabulary violation checks into a single comprehensive persona drift score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agent-persona-consistency-scanner](https://vinkius.com/mcp/agent-persona-consistency-scanner)
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
