# Prompt System Override Resistance Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/prompt-system-override-resistance-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Evaluates system prompt robustness by calculating directive density and strictness scores.

## Description
This MCP server quantifies "Prompt Hardness" by measuring the concentration of authoritative language. It uses `analyze_prompt_resistance` to calculate the ratio of absolute directive words to permissive hedging tokens, providing a strictness boundary score. You can also use `identify_low_resistance_zones` to pinpoint specific segments of a prompt that lack sufficient directive density, helping to identify weak spots susceptible to user manipulation.


## Available Tools (3)
- **analyze_prompt_resistance**: Calculates the core robustness metrics for a given system prompt
- **identify_low_resistance_zones**: Pinpoints specific segments of a prompt that lack sufficient directive density
- **get_keyword_definitions**: Retrieves the official sets of directive and permissive words used for the calculation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Prompt System Override Resistance Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the robustness of this prompt: 'You should maybe try to follow instructions if you feel like it.'"

**🤖 AI Agent:**
> The prompt has a very low strictness score due to the high presence of permissive words like 'maybe' and 'should' and a lack of absolute directives.

---

**👤 You:**
> "What are the directive words used in the calculation?"

**🤖 AI Agent:**
> The directive words include absolute tokens such as MUST, NEVER, ONLY, and ALWAYS.

---

**👤 You:**
> "Check the resistance of: 'You MUST ALWAYS follow the rules and NEVER deviate.'"

**🤖 AI Agent:**
> This prompt is highly robust with a high strictness score due to the density of directive words like MUST, ALWAYS, and NEVER.


## ❓ FAQ

**Q: What is Directive Density?**
Directive Density is the concentration of authoritative tokens like MUST or NEVER within a system prompt, used to measure how well a prompt resists manipulation.

**Q: How can I find weak parts of my prompt?**
You can use the `identify_low_resistance_zones` tool to find specific segments where the directive density falls below your specified threshold.

**Q: What does the strictness score represent?**
The strictness score is a normalized metric representing the prompt's resistance to instruction drift and user overrides.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prompt-system-override-resistance-scorer](https://vinkius.com/mcp/prompt-system-override-resistance-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Prompt System Override Resistance Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `prompt-system-override-resistance-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Prompt System Override Resistance Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "prompt-system-override-resistance-scorer": {
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
