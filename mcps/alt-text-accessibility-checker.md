# Alt-Text Accessibility Checker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alt-text-accessibility-checker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [web-development](../categories/web-development.md)

Validate image alt-text against WCAG standards for length, redundancy, and descriptiveness.

## Description
The Alt-Text Accessibility Checker ensures web images meet accessibility requirements. Use `check_length` to verify character counts, `analyze_redundancy` to remove 'image of' phrases, and `determine_image_role` to classify images as informative or decorative.


## Available Tools (5)
- **analyze_redundancy**: Identify redundant phrases in alt-text
- **check_length**: Check if alt-text length is within recommended bounds
- **determine_image_role**: Classify image as informative or decorative
- **evaluate_descriptiveness**: Calculate descriptiveness score
- **identify_duplicates**: Detect duplicate alt-text on a page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alt-Text Accessibility Checker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if 'A golden retriever running in grass' is a good alt-text for length."

**🤖 AI Agent:**
> The character count is 37, which falls within the recommended range.

---

**👤 You:**
> "Does the text 'picture of a cat' pass redundancy checks?"

**🤖 AI Agent:**
> No, it contains the redundant phrase 'picture of'.

---

**👤 You:**
> "Classify an image with alt-text '' (empty string)."

**🤖 AI Agent:**
> The image is classified as decorative.


## ❓ FAQ

**Q: How does it check for redundancy?**
It uses `analyze_redundancy` to scan for phrases like 'picture of' or 'graphic showing'.

**Q: Can I check multiple images at once?**
Yes, use `identify_duplicates` with a list of alt-text strings to find repeated descriptions on a page.

**Q: What is the recommended length for alt-text?**
The `check_length` tool verifies if your text stays within the optimal character range defined by WCAG guidelines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alt-text-accessibility-checker](https://vinkius.com/mcp/alt-text-accessibility-checker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alt-Text Accessibility Checker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `alt-text-accessibility-checker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alt-Text Accessibility Checker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alt-text-accessibility-checker": {
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
