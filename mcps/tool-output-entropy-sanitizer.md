# Tool Output Entropy Sanitizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tool-output-entropy-sanitizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detects and redacts high-entropy strings like API keys from tool outputs.

## Description
The Tool Output Entropy Sanitizer is a security-focused MCP server designed to prevent sensitive data leakage into LLM context windows. By implementing a sliding-window analysis, the `sanitize_text_output` tool scans input strings for segments that exceed an entropy threshold of 4.5. It uses deterministic character frequency analysis to identify high-entropy patterns characteristic of API keys, passwords, or encoded payloads. The server also provides `evaluate_segment_entropy` to audit specific substrings and `verify_window_bounds` to ensure window sizes remain within the operational bounds of 16 to 64 characters. When a secret is detected, it is replaced with a structured redaction pattern like `[REDACTED_HIGH_ENTROPY:length]`, preserving the structural context for the AI while protecting sensitive information.


## Available Tools (3)
- **evaluate_segment_entropy**: Input must be at least 16 characters long.

Audits the randomness of a specific piece of text
- **sanitize_text_output**: Returns the sanitized text and metadata about redactions.

Sanitizes text by redacting high-entropy segments
- **verify_window_bounds**: Ensures a proposed window size adheres to constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tool Output Entropy Sanitizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Sanitize this string: 'My API key is ABC123XYZ789! and my name is John'."

**🤖 AI Agent:**
> The sanitized text is: 'My API key is [REDACT_HIGH_ENTROPY:15] and my name is John'. Redacted count: 1.

---

**👤 You:**
> "What is the entropy score for 'password1234567890abcde'?"

**🤖 AI Agent:**
> The entropy score for the segment is 3.8, which is below the high-entropy threshold.

---

**👤 You:**
> "Is a window size of 10 valid for entropy analysis?"

**🤖 AI Agent:**
> No, the window size is invalid. The `verify_window_bounds` tool indicates it must be between 16 and 64 characters.


## ❓ FAQ

**Q: How does the sanitizer identify secrets?**
The server uses Shannon entropy calculation. If a window of text has an entropy score above 4.5, it is flagged as high-risk and redacted.

**Q: What happens to the redacted text?**
The high-entropy segment is replaced with a redaction pattern in the format `[REDACTED_HIGH_ENTROPY:length]`, where length is the original character count.

**Q: Can I check a specific string without redacting it?**
Yes, you can use the `evaluate_segment_entropy` tool to get the entropy score and high-entropy flag for a specific text segment without modifying the input.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tool-output-entropy-sanitizer](https://vinkius.com/mcp/tool-output-entropy-sanitizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tool Output Entropy Sanitizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tool-output-entropy-sanitizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tool Output Entropy Sanitizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tool-output-entropy-sanitizer": {
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
