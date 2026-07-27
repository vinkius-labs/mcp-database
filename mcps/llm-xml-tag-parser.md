# LLM XML Tag Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/llm-xml-tag-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-extraction](../categories/data-extraction.md)

Extract and validate content within XML-style tags from LLM outputs.

## Description
The LLM XML Tag Parser MCP server provides a deterministic way to parse structured data embedded in unstructured text. It is specifically designed for handling the output of models like Claude that use XML tags (e.g., ``, ``) to separate reasoning from final responses. Using robust regex-based extraction and depth tracking, it can handle nested tags and verify structural integrity. You can use `extract_single_tag` to find specific blocks, `extract_all_tags` to retrieve all instances of a tag, or `validate_tag_integrity` to ensure your XML structure is balanced.


## Available Tools (3)
- **extract_all_tags**: Extract all top-level occurrences of a specific XML tag
- **extract_single_tag**: Extract the first occurrence of a specific XML tag
- **validate_tag_integrity**: Validate the integrity of XML tag nesting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LLM XML Tag Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the reasoning from this output: <think>I should check the weather.</think><answer>The weather is sunny.</answer>"

**🤖 AI Agent:**
> I should check the weather.

---

**👤 You:**
> "Check if these tags are balanced: <data><item>1</item></data>"

**🤖 AI Agent:**
> The tag integrity is valid, and the nesting depth was 1.

---

**👤 You:**
> "Find all instances of the 'note' tag in: <note>First</note><other>Text</other><note>Second</note>"

**🤖 AI Agent:**
> ['First', 'Second']


## ❓ FAQ

**Q: How does the parser handle nested tags?**
The parser uses an integer depth counter. When it encounters an opening tag, it increments the counter; when it finds a closing tag, it decrements it. This ensures that `extract_all_tags` correctly identifies fully closed pairs even in complex structures.

**Q: Can I use this to validate if my prompt output is well-formed?**
Yes, by using the `validate_tag_integrity` tool, you can check if every opening tag has a corresponding closing tag and verify that the nesting depth is balanced.

**Q: What happens if a tag is not found?**
If you use `extract_single_tag` and the target tag does not exist in the input string, the tool will return null for the extracted content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/llm-xml-tag-parser](https://vinkius.com/mcp/llm-xml-tag-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LLM XML Tag Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `llm-xml-tag-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LLM XML Tag Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "llm-xml-tag-parser": {
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
