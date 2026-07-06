# Regex to NFA/DFA Visualizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regex-to-nfadfa-visualizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automata-theory](../categories/automata-theory.md)

Convert regular expressions to NFA and DFA structures with detailed state transition tables.

## Description
This MCP server provides a way to visualize formal language theory. Use `regex_to_nfa` to transform any regular expression into a Nondeterministic Finite Automaton using Thompson's construction. You can then use `nfa_to_dfa` to convert that NFA into a Deterministic Finite Automaton via subset construction. Additionally, the `check_language_finiteness` tool allows you to determine if the language represented by an automaton is finite or infinite by analyzing its cycles.


## Available Tools (2)
- **nfa_to_dfa**: Converts an NFA to a DFA
- **regex_to_nfa**: g., "abc") and get the NFA structure with states and transitions.

Converts a regex pattern to an NFA


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regex to NFA/DFA Visualizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the regex (a|b)* to an NFA."

**🤖 AI Agent:**
> The NFA for (a|b)* includes states s0, s1, and s2, with transitions for 'a', 'b', and epsilon.

---

**👤 You:**
> "Is the language defined by this NFA finite? {"states": ["s0", "s1"], "transitions": [{"from_state": "s0", "symbol": "a", "to_states": ["s0"]}]}"

**🤖 AI Agent:**
> No, the language is infinite because there is a cycle in the automaton that can reach an accepting state.

---

**👤 You:**
> "Transform this NFA to a DFA. {"alphabet": ["a"], "states": ["s0", "s1"], "start_state": "s0", "accept_states": ["s1"], "transitions": [{"from_state": "s0", "symbol": "a", "to_states": ["s1"]}]}"

**🤖 AI Agent:**
> The resulting DFA contains states representing the epsilon closures of the original NFA states, with unambiguous transitions for each alphabet symbol.


## ❓ FAQ

**Q: How do I convert a regex to an NFA?**
Use the `regex_to_nfa` tool by providing your regular expression pattern as input.

**Q: Can I check if a language is infinite?**
Yes, use the `check_language_finiteness` tool with an automaton definition to see if it contains reachable cycles.

**Q: Does this support DFA conversion?**
Yes, the `nfa_to_dfa` tool performs subset construction to transform NFA structures into DFAs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regex-to-nfadfa-visualizer](https://vinkius.com/mcp/regex-to-nfadfa-visualizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Regex to NFA/DFA Visualizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `regex-to-nfadfa-visualizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Regex to NFA/DFA Visualizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "regex-to-nfadfa-visualizer": {
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
