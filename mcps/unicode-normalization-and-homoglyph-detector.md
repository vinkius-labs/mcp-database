# Unicode Normalization and Homoglyph Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unicode-normalization-and-homoglyph-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security](../categories/security.md)

Detects malicious Unicode homoglyph attacks and identifies invisible characters in strings.

## Description
This MCP server provides specialized tools to identify security threats within Unicode strings. It detects malicious homoglyph substitutions (such as Cyrillic 'а' vs Latin 'a') and flags invisible zero-width characters that are often used to bypass code reviews or text filters. Using `analyze_string_security`, you can perform a high-level assessment of any input string. The server also provides `detect_hidden_characters` to find non-printing codepoints and `inspect_homoglyph_substitutions` to isolate visual spoofing attempts. All detection is performed via deterministic integer codepoint comparison, ensuring reliable security analysis.


## Available Tools (3)
- **inspect_homoglyph_substitutions**: Isolates and reports only the visual substitutions found in a string
- **analyze_string_security**: Provides a high-level security assessment of a provided string
- **detect_hidden_characters**: Scans for the presence of invisible or zero-width characters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unicode Normalization and Homoglyph Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this string for security threats: 'pаypal.com'"

**🤖 AI Agent:**
> The string 'pаypal.com' is unsafe because it contains a Cyrillic 'а' instead of a Latin 'a', which is a homoglyph substitution.

---

**👤 You:**
> "Are there any hidden characters in this text?"

**🤖 AI Agent:**
> The scan found one hidden character at position 5 (U+200B).

---

**👤 You:**
> "Check if 'hello' has any visual substitutions."

**🤖 AI Agent:**
> No visual substitutions were detected in the string 'hello'.


## ❓ FAQ

**Q: What are homoglyph attacks?**
Homoglyph attacks occur when visually similar characters from different scripts (like Cyrillic or Greek) are used to impersonate Latin characters, potentially creating deceptive URLs or usernames.

**Q: How does the tool detect hidden characters?**
The `detect_hidden_characters` tool scans for specific Unicode codepoints that have no visual width, such as U+200B (Zero Width Space), which are often used to hide malicious payloads.

**Q: Can I normalize strings using this server?**
Yes, when using `analyze_string_security`, you can set the `applyNormalization` parameter to true to receive the string in its standardized NFC (Normalization Form Canonical Composition) format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unicode-normalization-and-homoglyph-detector](https://vinkius.com/mcp/unicode-normalization-and-homoglyph-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unicode Normalization and Homoglyph Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `unicode-normalization-and-homoglyph-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unicode Normalization and Homoglyph Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unicode-normalization-and-homoglyph-detector": {
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
