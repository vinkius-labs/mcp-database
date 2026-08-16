# RoboHash MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/robohash)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Generate unique robot, monster, or kitten avatars from any text string — perfect for profile pictures and placeholders.

## Description
RoboHash provides a fun and easy way to generate unique images from any text. Whether you need an avatar for a new user or a placeholder for a project, RoboHash creates consistent, high-quality visuals based on the hash of your input string.

### What you can do

- **Avatar Generation** — Create unique robots, monsters, kittens, humans, or gorillas from names, emails, or random strings.
- **Visual Styles** — Choose from 6 distinct sets (Robots, Monsters, Heads, Kittens, Humans, Gorillas) to match your project's aesthetic.
- **Custom Backgrounds** — Add generated backgrounds (bg1 or bg2) to make your avatars stand out.
- **Flexible Sizing** — Specify exact dimensions (e.g., 200x200, 500x500) for your generated images.
- **Format Support** — Export your generated assets in PNG, JPG, or BMP formats.

### How it works

1. Subscribe to this server
2. Enter your RoboHash API identifier
3. Start generating avatars directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — quickly generate unique user avatars for testing or production environments without hosting assets.
- **Designers** — create placeholder characters for UI/UX mockups instantly.
- **Community Managers** — provide fun, automated profile pictures for members based on their usernames.


## Available Tools (1)
- **generate_robohash_avatar**: Generate a unique RoboHash image URL from text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RoboHash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a robot image for the text 'mcp-user-123'."

**🤖 AI Agent:**
> I've generated a unique robot for you! You can view it here: https://robohash.org/mcp-user-123.png?set=set1

---

**👤 You:**
> "Create a kitten avatar for 'hello@world.com' with a background in 400x400 size."

**🤖 AI Agent:**
> Here is your kitten avatar with a background: https://robohash.org/hello@world.com.png?set=set4&bgset=bg1&size=400x400

---

**👤 You:**
> "Generate a monster avatar for 'ProjectAlpha' in JPG format."

**🤖 AI Agent:**
> I've created a monster avatar for ProjectAlpha in JPG format: https://robohash.org/ProjectAlpha.jpg?set=set2


## ❓ FAQ

**Q: How do I change the type of character generated (e.g., from a robot to a kitten)?**
You can use the `set` parameter in the `generate_robohash_avatar` tool. Choose 'set1' for robots, 'set2' for monsters, 'set4' for kittens, and so on.

**Q: Can I specify the exact dimensions of the image?**
Yes! Use the `size` parameter in the format 'WxH' (e.g., '300x300') when calling the `generate_robohash_avatar` tool to get the exact resolution you need.

**Q: What does the 'gravatar' option do?**
The `gravatar` parameter allows the tool to check if the provided text (like an email) has a Gravatar associated with it. If 'yes', it will return the Gravatar instead of a RoboHash if one exists.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/robohash](https://vinkius.com/ai-agent-connect/robohash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RoboHash** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `robohash` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RoboHash** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "robohash": {
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
