# Vigenère Cipher Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vigenere-cipher-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Deterministic Vigenère cipher encoder and decoder that preserves text formatting.

## Description
This MCP server provides a deterministic engine for performing Vigenère encryption and decryption. It allows AI agents to transform text using a keyword while strictly maintaining original spaces, punctuation, and casing. The engine uses `transform_text` to process strings, `validate_keyword` to ensure keyword integrity, and `get_cipher_summary` to analyze keyword characteristics. It is designed to handle keyword repetition and modular arithmetic precisely, ensuring that non-alphabetic characters do not disrupt the cipher stream.


## Available Tools (3)
- **get_cipher_summary**: Provides metadata about the strength and characteristics of a keyword
- **transform_text**: Performs Vigenère encryption or decryption on the provided text using a keyword
- **validate_keyword**: Validates if a keyword is suitable for the Vigenère cipher


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vigenère Cipher Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Encode the text 'Hello World!' using the keyword 'KEY'."

**🤖 AI Agent:**
> Rijss Gspvh!

---

**👤 You:**
> "Decode 'Rijss Gspvh!' using the keyword 'KEY'."

**🤖 AI Agent:**
> Hello World!

---

**👤 You:**
> "Is the keyword '123' valid for the Vigenère cipher?"

**🤖 AI Agent:**
> No, the keyword must consist entirely of alphabetic characters.


## ❓ FAQ

**Q: Does this tool preserve my original text formatting?**
Yes, the `transform_text` tool preserves all spaces, punctuation, and casing from your original input.

**Q: How can I check if my keyword is valid?**
You can use the `validate_keyword` tool to ensure your keyword consists only of alphabetic characters.

**Q: What information can I get about my keyword?**
The `get_cipher_summary` tool provides the length, number of unique letters, and pattern strength of your keyword.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vigenere-cipher-engine](https://vinkius.com/ai-agent-connect/vigenere-cipher-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vigenère Cipher Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vigenere-cipher-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vigenère Cipher Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vigenere-cipher-engine": {
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
