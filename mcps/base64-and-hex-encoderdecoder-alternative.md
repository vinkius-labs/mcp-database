# Base64 and Hex Encoder/Decoder Alternative MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/base64-and-hex-encoderdecoder-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Encode and decode strings between Base64, Base64URL, and Hexadecimal formats with byte size calculation.

## Description
This MCP server provides a precise utility for transforming text across multiple encoding schemes. It allows AI agents to perform reliable conversions between plain text and Base64, Base64URL (URL-safe), and Hexadecimal formats. Beyond simple conversion, the server includes functionality to calculate the exact byte size of any payload using UTF-8 encoding, which is essential for managing data limits in API requests or database storage. Using tools like `encode_base64`, `decode_hex`, or `get_byte_size`, agents can verify string integrity and prepare data for web-safe transmission without relying on external APIs.


## Available Tools (7)
- **decode_hex**: Decodes a Hexadecimal string
- **get_byte_size**: Calculates the byte size of a string
- **decode_base64**: Decodes a Base64 string
- **decode_base64url**: Decodes a Base64URL string
- **encode_base64**: Encodes a string to Base64
- **encode_base64url**: Encodes a string to Base64URL
- **encode_hex**: Encodes a string to Hexadecimal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Base64 and Hex Encoder/Decoder Alternative** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert the word 'Hello' to Base64."

**🤖 AI Agent:**
> SGVsbG8=

---

**👤 You:**
> "What is the hexadecimal representation of 'abc'?"

**🤖 AI Agent:**
> 616263

---

**👤 You:**
> "How many bytes is the string 'Vinkius'?"

**🤖 AI Agent:**
> 7


## ❓ FAQ

**Q: Does this server require an API key?**
No, this server performs all mathematical conversions locally. No external APIs or authentication keys are required to use the encoding tools.

**Q: How can I check the size of my encoded payload?**
You can use the `get_byte_size` tool to calculate exactly how many bytes a string occupies in UTF-8 encoding.

**Q: Is Base64URL different from standard Base64?**
Yes, Base64URL is a variant of Base64 that replaces characters like '+' and '/' with '-' and '_' to ensure the string is safe for use in URLs.

**Q: Is Base64URL different from standard Base64?**
Yes, Base64URL is a variant of Base64 that replaces characters like '+' and '/' with '-' and '_' to ensure the string is safe for use in URLs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/base64-and-hex-encoderdecoder-alternative](https://vinkius.com/ai-agent-connect/base64-and-hex-encoderdecoder-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Base64 and Hex Encoder/Decoder Alternative** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `base64-and-hex-encoderdecoder-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Base64 and Hex Encoder/Decoder Alternative** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "base64-and-hex-encoderdecoder-alternative": {
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
