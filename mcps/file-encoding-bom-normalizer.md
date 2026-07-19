# File Encoding & BOM Normalizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/file-encoding-bom-normalizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Detects and removes Byte Order Marks (BOM) and normalizes file encodings and line endings to a standard UTF-8 LF format.

## Description
The File Encoding & BOM Normalizer is a specialized utility for maintaining consistent file encoding and line ending standards across development environments. It prevents subtle runtime parser errors caused by Byte Order Marks (B/BOM) or mixed line endings (CRLF vs LF). Using the `identify_encoding_bom` tool, you can detect exact byte signatures for UTF-8, UTF-16 LE, and UTF-16 BE at the start of any file. The `inspect_line_endings` tool allows you to check if a file uses consistent LF or CRLF sequences. For larger scale changes, use `preview_normalization_stats` to calculate exactly how many bytes would be removed during a normalization process. Finally, `generate_normalized_payload` provides the clean, normalized text content of a file, stripped of BOM and converted to standard UTF-8 with LF line endings.


## Available Tools (4)
- **inspect_line_endings**: Check for consistent line endings in a file
- **generate_normalized_payload**: Generate the normalized text content of a file
- **identify_encoding_bom**: Identify the BOM signature at the start of a file
- **preview_normalization_stats**: Preview the impact of normalization on a file


## 💬 Prompt Examples

Here are some examples of how you can interact with the **File Encoding & BOM Normalizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if this file has a BOM signature."

**🤖 AI Agent:**
> The `identify_encoding_bom` tool has detected a UTF-8 BOM signature at the start of the file.

---

**👤 You:**
> "What are the line endings in this file?"

**🤖 AI Agent:**
> The `inspect_line_endings` tool reports that the file uses CRLF line endings.

---

**👤 You:**
> "Show me how many bytes would be removed during normalization."

**🤖 AI Agent:**
> The `preview_normalization_stats` tool indicates that 4 bytes would be removed to normalize the file.


## ❓ FAQ

**Q: What is a Byte Order Mark (BOM)?**
A BOM is a specific sequence of bytes at the beginning of a file that indicates how characters are encoded. Detecting and removing it is critical to prevent parser errors in many modern tools.

**Q: How can I check for mixed line endings?**
You can use the `inspect_line_endings` tool to scan a file and determine if it uses LF, CRLF, or mixed line endings.

**Q: Can I preview the changes before applying them?**
Yes, you can use `preview_normalization_stats` to see exactly how many bytes would be removed (such as BOM signatures or CRLF sequences) during the normalization process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/file-encoding-bom-normalizer](https://vinkius.com/mcp/file-encoding-bom-normalizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **File Encoding & BOM Normalizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `file-encoding-bom-normalizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **File Encoding & BOM Normalizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "file-encoding-bom-normalizer": {
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
