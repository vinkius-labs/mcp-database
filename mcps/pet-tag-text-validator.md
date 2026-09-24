# Pet Tag Text Validator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-tag-text-validator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Measure and validate character counts for pet tag engravings.

## Description
This MCP server provides tools to ensure pet identification tag messages fit within physical engraving limits. Use `get_text_metrics` to calculate character counts and whitespace, `validate_tag_fit` to check if a message fits a specific capacity, `check_language_compliance` to ensure text uses only allowed English characters, and `get_bulk_tag_analysis` to compare multiple message options at once.


## Available Tools (4)
- **check_language_compliance**: Verifies that the provided text strictly adheres to English language character requirements
- **get_bulk_tag_analysis**: Analyzes a list of multiple potential tag messages to find the best fit for a given capacity
- **get_text_metrics**: Calculates the total length and provides basic character statistics for a specific string of text
- **validate_tag_fit**: Determines if a specific text string will physically fit on a tag based on a predefined capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Tag Text Validator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many characters are in 'Buddy - 555-0123'?"

**🤖 AI Agent:**
> The text 'Buddy - 555-0123' contains 16 characters.

---

**👤 You:**
> "Will 'Max' fit on a tag with a 2 character limit?"

**🤖 AI Agent:**
> No, 'Max' has 3 characters and exceeds the limit of 2.

---

**👤 You:**
> "Is '🐶 Buddy' a valid tag message?"

**🤖 AI Agent:**
> No, the message contains invalid characters that are not part of the supported English set.


## ❓ FAQ

**Q: Does the character count include spaces?**
Yes, spaces are counted as characters because they occupy physical space on the engraved tag.

**Q: Can I use characters other than English?**
No, the system only supports the English alphabet and standard English punctuation to ensure high-quality engraving.

**Q: How do I check if multiple messages will fit?**
You can use the `get_bulk_tag_analysis` tool to evaluate a list of potential messages against a specific capacity limit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-tag-text-validator](https://vinkius.com/en/ai-agent-connect/pet-tag-text-validator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Tag Text Validator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-tag-text-validator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Tag Text Validator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-tag-text-validator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
