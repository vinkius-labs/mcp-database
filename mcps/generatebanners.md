# GenerateBanners MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/generatebanners)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Create professional ad banners and social media graphics automatically with templates that match your brand guidelines.

## Description
Connect your **GenerateBanners.com** account to any AI agent and take full control of your automated visual content creation and dynamic banner rendering through natural conversation.

### What you can do

- **Template Orchestration** — List all your image templates and retrieve detailed technical metadata about layers and dimensions programmatically
- **Automated Rendering** — Generate new banners and images by dynamically overriding text and image layers directly from your AI agent
- **Project Navigation** — List and manage your template projects to maintain a structured and organized visual asset library
- **Usage Intelligence** — Monitor remaining generation credits and plan details to ensure uninterrupted visual operations
- **Instant Deployment** — Retrieve real-time URLs for rendered banners for immediate use in social media, email, or web content

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your GenerateBanners.com account settings
3. Start rendering automated visuals from Claude, Cursor, or any MCP client

No more manual editing of images or slow design cycles. Your AI acts as your dedicated graphic production assistant.

### Who is this for?

- **Marketing Managers** — instantly automate the creation of personalized social media and email banners using natural language
- **E-commerce Owners** — scale product image generation with dynamic text and price overlays without leaving your workspace
- **Content Automators** — integrate automated image rendering into custom marketing stacks and data-driven workflows


## Available Tools
- **check_gb_status**: Verify connectivity
- **create_project**: Create a project
- **delete_project**: Delete a project
- **get_account**: Get account info
- **get_project**: Get project details
- **get_template**: Get template details
- **list_categories**: List categories
- **list_projects**: List projects
- **list_templates**: List templates
- **render_batch**: Render batch banners
- **render_template**: Render a banner
- **search_templates**: Search templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GenerateBanners** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my image templates in GenerateBanners."

**🤖 AI Agent:**
> I've retrieved your templates. You have 5 designs available, including 'Social Media Promo' (ID: 123) and 'Email Header' (ID: 456). Which one would you like to use for a new render?

---

**👤 You:**
> "Render a banner using template '123' with text '20% OFF' and a new background image."

**🤖 AI Agent:**
> Banner rendered! I've applied the '20% OFF' override and updated the background image as requested. You can view your new asset here: [link].

---

**👤 You:**
> "Check my GenerateBanners credit balance."

**🤖 AI Agent:**
> You currently have 850 generation credits remaining on your account. Your plan resets on the 1st of next month.


## ❓ FAQ

**Q: How do I find my API Key?**
Log in to your GenerateBanners.com account, navigate to your **Account Settings** or **API** section, and copy your unique key.

**Q: Can I override multiple layers at once?**
Yes! The `render_template` tool accepts a JSON string in `overrides_json` where you can provide multiple key-value pairs for different layers.

**Q: How do I track my remaining credits?**
Use the `get_account_info` tool to retrieve your current credit balance and plan limitations directly through your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/generatebanners](https://vinkius.com/mcp/generatebanners)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GenerateBanners** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `generatebanners` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GenerateBanners** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "generatebanners": {
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
