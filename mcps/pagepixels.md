# PagePixels MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pagepixels)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Capture website screenshots and generate visual previews programmatically with an API that handles rendering at any resolution.

## Description
### What you can do
- **Automated Screenshots**: Take high-quality screenshots of any URL.
- **Render Custom HTML**: Capture images of custom HTML generated on the fly.
- **Manage Configurations**: Create and update scheduled screenshot configurations for continuous monitoring.

### How it works
1. Sign up for PagePixels and generate an API Token.
2. Add the token to the integration settings.
3. Ask your AI Agent to take screenshots or manage your capturing configs effortlessly.

### Who is this for?
Ideal for developers, designers, and marketers who need to automate visual testing, track competitor websites, or generate dynamic images via AI agents.


## Available Tools (8)
- **delete_screenshot_config**: Delete a screenshot configuration
- **get_screenshot_config**: Get a specific screenshot configuration by ID
- **list_screenshot_configs**: List all screenshot configurations
- **quick_snap**: Takes a quick screenshot of a URL
- **quick_snap_with_options**: Takes a screenshot of a URL with advanced options
- **snap_custom_html**: Takes a screenshot of custom HTML
- **update_screenshot_config**: Update an existing screenshot configuration
- **create_screenshot_config**: Create a new screenshot configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PagePixels** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Take a full page screenshot of https://example.com."

**🤖 AI Agent:**
> I have successfully requested a full page screenshot for https://example.com.

---

**👤 You:**
> "List all my screenshot configurations."

**🤖 AI Agent:**
> Here are all your active screenshot configurations in PagePixels.

---

**👤 You:**
> "Render this HTML and take a screenshot."

**🤖 AI Agent:**
> The HTML has been rendered and the screenshot is available at the provided URL.


## ❓ FAQ

**Q: Does the AI agent store the screenshots?**
No, the AI agent uses PagePixels to generate the screenshots, which are stored securely by the PagePixels service and provided as URLs to the agent.

**Q: Can I capture full pages?**
Yes! The AI agent can use advanced options to instruct PagePixels to capture the entire height of the webpage.

**Q: Are there limits on screenshot generation?**
Limits depend strictly on your active PagePixels subscription plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pagepixels](https://vinkius.com/mcp/pagepixels)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PagePixels** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pagepixels` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PagePixels** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pagepixels": {
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
