# Regex Extractor Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/regex-extractor-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Stop LLM hallucination when extracting data. Run pure Regex across massive text blocks and guarantee 100% accurate array extraction without missing a single match.

## Description
LLMs often struggle with strict pattern matching, hallucinating data that isn't there or missing complex nested structures. This MCP brings pure, deterministic JavaScript RegExp evaluation to your agent.

### The Superpowers

- **Absolute Precision:** Extract emails, phone numbers, UUIDs, or custom tokens with 100% mathematical accuracy.
- **Zero Hallucination:** If the pattern isn't in the text, it returns nothing. It never invents a fake email address.
- **Native Speed:** Runs natively on the V8 engine at the edge.


## Available Tools (1)
- **regex_extractor_extract**: You provide the text and the regex, and this tool returns an exact array of matches without hallucinating or dropping items.

Extracts exact string matches from a large text using Regular Expressions (Regex)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regex Extractor Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract all UUIDs from this server log file."

**🤖 AI Agent:**
> ✅ **Extracted (2):**
- `123e4567-e89b-12d3-a456-426614174000`
- `987f6543-a21c-34f5-b678-998877665544`

---

**👤 You:**
> "Find every email ending in @vinkius.com in this text block."

**🤖 AI Agent:**
> ✅ **Matches Found:**
1. `admin@vinkius.com`
2. `sales-team@vinkius.com`

---

**👤 You:**
> "Validate if '192.168.1.255' matches a standard IPv4 address format."

**🤖 AI Agent:**
> ✅ **Validation Passed:** The string perfectly matches the IPv4 regular expression.


## ❓ FAQ

**Q: Why use this instead of asking the AI?**
LLMs can be tricked by obfuscated text and hallucinate missing numbers. RegExp is a mathematical guarantee.

**Q: Does it support custom flags?**
Yes, you can pass standard flags like 'g', 'i', or 'm' to modify the evaluation behavior.

**Q: Can I extract multiple complex patterns at once?**
Absolutely. The global flag extracts an array of all exact matches instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/regex-extractor-engine](https://vinkius.com/mcp/regex-extractor-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Regex Extractor Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `regex-extractor-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Regex Extractor Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "regex-extractor-engine": {
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
