# RenderForm MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/renderform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate dynamic images and social media graphics from templates with an API that personalizes visuals at scale for any campaign.

## Description
Empower your AI agent with the ability to generate high-quality images and PDFs using **RenderForm** templates. RenderForm provides a powerful REST API for visual automation, allowing you to orchestrate marketing assets, OpenGraph images, and dynamic documents through simple natural language commands.

### What you can do

- **Image Generation** — Render dynamic images for social media or marketing using template components and real-time data.
- **PDF Automation** — Generate documents and PDFs with custom layouts and dynamic variables programmatically.
- **Template Management** — List all available templates and retrieve detailed component structures to understand visual possibilities.
- **Asset & Project Oversight** — Manage fonts, logos, and uploaded assets to ensure consistent branding across all generated content.
- **Operational Monitoring** — Track system health, monitor render quotas, and retrieve request logs using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your RenderForm API Key from your dashboard
3. Start generating visual content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Marketers** — quickly generate varied social media assets without leaving your workspace.
- **Developers** — integrate automated image rendering into your app workflows without complex media processing logic.
- **Ops Teams** — streamline the generation of dynamic PDF reports and monitor rendering consumption directly within the chat.


## Available Tools (12)
- **check_api_status**: Check RenderForm API status
- **get_account_info**: Get account information and quotas
- **get_request_status**: Get the status of a render request
- **get_template_details**: Get details for a specific template
- **list_assets**: List uploaded assets
- **list_available_fonts**: List available fonts
- **list_logos**: List uploaded logos
- **list_projects**: List all projects
- **list_render_requests**: List recent render requests
- **list_templates**: List all available templates
- **render_image**: Render an image from a template
- **render_pdf**: Render a PDF document from a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RenderForm** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my image templates in RenderForm."

**🤖 AI Agent:**
> I've found your templates. You have 5 active designs including 'IG Post v1' (ID: ig_123) and 'Email Header'. Which one would you like to render?

---

**👤 You:**
> "Generate a social media banner for our Summer Sale campaign using the product showcase template."

**🤖 AI Agent:**
> Banner generated successfully. Template: "Product Showcase v3" (ID: tpl_8834). Dimensions: 1200x628px (Facebook/LinkedIn optimized). Dynamic fields populated: headline "Summer Sale - Up to 60% Off", product image (uploaded), brand colors applied, CTA button "Shop Now". Output format: PNG (high quality). Download URL generated. The template also auto-generated versions for Instagram (1080x1080) and Twitter (1600x900). All 3 variants saved to your project folder.

---

**👤 You:**
> "List all available templates in my account and show which ones have been used the most."

**🤖 AI Agent:**
> You have 28 templates. Top 5 by usage: "Social Media Post" (1,234 renders), "Email Header" (890 renders), "Product Card" (678 renders), "Certificate" (456 renders), "Invoice" (234 renders). 8 templates were created this month. Average renders per template: 127. Most popular format: PNG (72%), followed by PDF (18%) and JPG (10%). 3 templates have not been used in 60+ days and may be candidates for archival.


## ❓ FAQ

**Q: Can my AI automatically find my RenderForm templates?**
Yes! Use the `list_templates` tool. Your agent will respond with complete metadata for all your templates, including their IDs and descriptions in seconds.

**Q: How do I get an API key?**
Log in to your RenderForm dashboard and navigate to the **API Keys** tab in your account section to copy your unique secret key.

**Q: Can I use dynamic data for my images?**
Yes, you can pass a data object to the `render_image` tool to replace text, images, and colors in your templates programmatically via natural language.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/renderform](https://vinkius.com/mcp/renderform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RenderForm** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `renderform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RenderForm** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "renderform": {
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
