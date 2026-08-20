# Poetic Meter Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/poetic-meter-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Deterministic poetic meter and syllable analysis for English poetry.

## Description
This MCP server provides precise phonetic and rhythmic decomposition of English verse. Use `analyze_line` to obtain syllable counts, stress patterns, and meter classifications. You can also use `identify_meter_type` to categorize specific stress sequences or `detect_rhyme` to verify phonetic matches between lines. It accounts for complex linguistic rules like elision, syncope, and silent 'e' to ensure accuracy in meter identification and rhyme detection.


## Available Tools (3)
- **analyze_line**: Performs a deep phonetic and rhythmic decomposition of a single line of poetry
- **detect_rhyme**: Determines if two lines rhyme based on their phonetic endings
- **identify_meter_type**: Categorizes a sequence of stresses into a specific metrical name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Poetic Meter Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the meter of this line: 'Shall I compare thee to a summer's day?'"

**🤖 AI Agent:**
> The line is in iambic pentameter with 10 syllables.

---

**👤 You:**
> "Do 'heart' and 'part' rhyme?"

**🤖 AI Agent:**
> Yes, 'heart' and 'part' are a perfect rhyme.

---

**👤 You:**
> "What is the stress pattern for 'Double, double toil and trouble'?"

**🤖 AI Agent:**
> The stress pattern is trochaic tetrameter.


## ❓ FAQ

**Q: How does the tool handle silent letters?**
The tool follows CMU Pronouncing Dictionary standards, specifically accounting for silent 'e' and other phonetic rules to ensure syllable counts and stress patterns are accurate.

**Q: Can I check if two lines rhyme?**
Yes, you can use the `detect_rhyme` tool to compare the phonetic endings of two lines and determine if they constitute a perfect or slant rhyme.

**Q: What kind of meter can be identified?**
The server can identify standard English meters including iambic, trochaic, anapestic, dactylic, and spondaic patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/poetic-meter-analyzer](https://vinkius.com/ai-agent-connect/poetic-meter-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Poetic Meter Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `poetic-meter-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Poetic Meter Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "poetic-meter-analyzer": {
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
