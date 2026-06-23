# Carbonara MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/carbonara)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Transform code snippets into beautiful, high-quality images with syntax highlighting, custom themes, and window controls directly from your AI agent.

## Description
Connect **Carbonara** to your AI agent to generate professional, social-media-ready screenshots of your code. Perfect for documentation, tutorials, and sharing snippets with style.

### What you can do

- **Syntax Highlighting** — Render code in various languages with automatic detection or specific language mapping
- **Custom Themes** — Choose from popular themes like 'seti' to match your brand or preference
- **Window Styling** — Add macOS-style window controls (close/minimize/maximize) and choose between sharp or rounded window themes
- **Visual Effects** — Configure drop shadows, custom background colors, and padding for a polished look
- **Advanced Formatting** — Toggle line numbers, highlight specific lines of interest, and adjust font sizes or families

### How it works

1. Subscribe to this server
2. Provide your Carbonara instance Base URL
3. Ask your AI to "cook" any code snippet into a high-quality PNG image

### Who is this for?

- **Technical Writers** — Create consistent, beautiful code illustrations for blog posts and documentation
- **Developers** — Share clean, readable code snippets on social media or in team chats without messy copy-pasting
- **Educators** — Generate clear visual aids for programming tutorials and slides


## Available Tools (1)
- **cook_code_image**: Returns a base64 encoded PNG image.

Generate a beautiful image of a code snippet


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carbonara** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Cook a code image for this Python function using the 'seti' theme and include line numbers."

**🤖 AI Agent:**
> I've generated the image for your Python function. It features the 'seti' theme with visible line numbers for better readability. [Image Attached]

---

**👤 You:**
> "Create a high-resolution screenshot of this React component with a blue background and drop shadow."

**🤖 AI Agent:**
> Processing your React component... I've rendered it with a custom blue background and a soft drop shadow for a professional look. [Image Attached]

---

**👤 You:**
> "Generate a code snippet image for this SQL query, highlight lines 2 and 4, and add macOS window controls."

**🤖 AI Agent:**
> The SQL query has been 'cooked'. I've highlighted the requested lines and added the window controls as specified. [Image Attached]


## ❓ FAQ

**Q: Can I customize the syntax highlighting theme and font?**
Yes! You can use the `theme` parameter (e.g., 'seti') and `fontFamily` or `fontSize` to match your preferred style perfectly.

**Q: Is it possible to highlight specific lines of code in the image?**
Absolutely. Use the `selectedLines` parameter to provide a comma-separated list of line numbers (e.g., '3,5,6') that you want to emphasize.

**Q: Can I add window controls like the ones on macOS?**
Yes, by setting `windowControls` to true, the generated image will include the classic close, minimize, and maximize buttons.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/carbonara](https://vinkius.com/mcp/carbonara)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carbonara** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carbonara` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carbonara** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carbonara": {
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
