# Brand Voice Consistency Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brand-voice-consistency-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Audit copy samples against brand voice profiles for linguistic and stylistic alignment.

## Description
The Brand Voice Consistency Checker is an automated validator that ensures your copy adheres to a predefined brand identity. Using the `check_vocabulary` tool, you can identify prohibited language and track preferred terminology. The `check_syntax` tool evaluates structural integrity by checking sentence length ranges and punctuation rules like Oxford commas. Finally, `calculate_alignment` measures qualitative attributes such as lexical formality and readability grade levels. This MCP server acts as a bridge for AI agents to maintain brand integrity across all communications.


## Available Tools (3)
- **calculate_alignment**: Measures qualitative attributes like tone and readability
- **check_syntax**: Evaluates sentence structure and punctuation against brand rules
- **check_vocabulary**: Checks for banned words and tracks preferred brand terminology


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brand Voice Consistency Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check this text for brand violations: 'Our amazing product is the best, buy it now!!!' with banned words ['amazing', 'best'] and target contraction ratio 0.1."

**🤖 AI Agent:**
> The text contains 2 banned word matches: 'amazing' and 'best'. The actual contraction ratio is 0.0.

---

**👤 You:**
> "Evaluate the syntax of: 'Hello. This is a test.' with minWords 5 and maxWords 10."

**🤖 AI Agent:**
> The sentence length deviation score is high because the sentences are below the minimum word count requirement.

---

**👤 You:**
> "How does the text 'Professionalism is key.' compare to a target formality of 90 and readability grade of 12?"

**🤖 AI Agent:**
> The tone consistency score is 85, and the readability level delta is +2.0.


## ❓ FAQ

**Q: How does the vocabulary check work?**
The `check_vocabulary` tool scans your text for any words listed in your banned list and counts the occurrences of preferred terms.

**Q: Can I check for punctuation rules?**
Yes, the `check_syntax` tool allows you to define rules for Oxford commas and maximum exclamation mark usage.

**Q: What is the purpose of linguistic alignment?**
The `calculate_alignment` tool measures how closely your text matches target formality and readability grade levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brand-voice-consistency-checker](https://vinkius.com/mcp/brand-voice-consistency-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Brand Voice Consistency Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brand-voice-consistency-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Brand Voice Consistency Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brand-voice-consistency-checker": {
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
