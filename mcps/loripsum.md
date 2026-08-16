# Loripsum MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/loripsum)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate professional placeholder text (Lorem Ipsum) with customizable HTML formatting, lists, and headers for your mockups.

## Description
Connect the **Loripsum** engine to your AI agent to instantly generate placeholder text for web development, design mockups, and content strategy. No more copying and pasting from external websites; let your AI handle the layout text generation directly.

### What you can do

- **Custom Lengths** — Generate specific numbers of paragraphs with lengths ranging from short to very long.
- **Rich Formatting** — Automatically include HTML tags like ``, ``, and `` using the decorate option.
- **Structural Elements** — Generate complex structures including unordered lists (``), ordered lists (``), and description lists (``).
- **Technical Content** — Add blockquotes, code samples, and headers to test your CSS and layout responsiveness.
- **Plain Text Mode** — Switch between HTML and clean plaintext for simple copy-pasting into non-web environments.

### How it works

1. Subscribe to this server
2. Use the `generate_loripsum_text` tool to specify your requirements
3. Receive formatted placeholder text ready for use in your project

### Who is this for?

- **Web Developers** — quickly fill new components with realistic HTML structures to test styling
- **UI/UX Designers** — generate varied content lengths to verify how layouts handle different text volumes
- **Content Strategists** — create draft wireframes with structured text without manual formatting


## Available Tools (1)
- **generate_loripsum_text**: Returns HTML by default unless plaintext is requested.

Generate placeholder text (Lorem Ipsum)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loripsum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate 3 medium paragraphs of Lorem Ipsum with bold formatting and links."

**🤖 AI Agent:**
> I've generated 3 medium paragraphs for you. The text includes `<strong>` tags for decoration and random `<a>` links as requested. Would you like me to add any headers or lists as well?

---

**👤 You:**
> "Give me 5 short paragraphs of placeholder text in plaintext mode."

**🤖 AI Agent:**
> Here are 5 short paragraphs of Lorem Ipsum in plaintext format, ready for you to copy and paste without any HTML tags.

---

**👤 You:**
> "Generate a Lorem Ipsum response with an unordered list and code samples."

**🤖 AI Agent:**
> I've created the content with an unordered list (`<ul>`) and code blocks (`<code>`). This should help you test the technical layout of your page.


## ❓ FAQ

**Q: Can I generate plain text instead of HTML for my mockups?**
Yes! Simply set the `plaintext` parameter to true when calling the `generate_loripsum_text` tool. The server will return clean text without any HTML tags.

**Q: How do I add lists or headers to the generated text?**
You can use the optional boolean parameters like `ul` (unordered lists), `ol` (ordered lists), or `headers` in the `generate_loripsum_text` tool to include these structural elements in your output.

**Q: Is there a way to avoid potentially offensive words in the placeholder text?**
Yes, the `generate_loripsum_text` tool includes a `prude` option. When enabled, it uses a version of the text that removes words that might be considered offensive.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/loripsum](https://vinkius.com/ai-agent-connect/loripsum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loripsum** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `loripsum` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loripsum** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loripsum": {
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
