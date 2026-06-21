# Easelly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/easelly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Design infographics and visual reports using templates and a drag-and-drop editor that makes data storytelling simple.

## Description
Connect your **Easelly** Pro account to any AI agent and take full control of your visual content creation and automated infographic workflows through natural conversation.

### What you can do

- **Design Orchestration** — List and manage all infographics in your Easel.ly account and retrieve detailed metadata about themes and objects programmatically
- **Automated Export** — Programmatically generate high-fidelity PDF, JPG, or PNG versions of your designs for immediate use in marketing or education
- **Structure Intelligence** — Access the raw JSON representation of any infographic to understand layer hierarchies and content distributions programmatically
- **Dynamic Creation** — Create new infographics from scratch or existing templates and update content programmatically directly through your agent
- **Visual Maintenance** — Programmatically delete or update infographic metadata to maintain a clean and structured visual asset library

### How it works

1. Subscribe to this server
2. Retrieve your **Pro API Key** from your Easel.ly account settings
3. Start generating and managing professional infographics from Claude, Cursor, or any MCP client

No more manual editing for every small visual change. Your AI acts as your dedicated graphic production assistant and visual content coordinator.

### Who is this for?

- **Content Marketers** — instantly generate image versions of infographics for social media posts using natural language commands
- **Educators & Researchers** — automate the creation of data visualizations and export PDFs without leaving your workspace
- **Developers** — integrate automated infographic design and export features into custom internal tools through simple AI queries


## Available Tools
- **create_infographic**: Create a new infographic
- **generate_image**: Generate an image for an infographic
- **generate_json**: Get infographic structure in JSON
- **generate_pdf**: Generate a PDF for an infographic
- **list_infographics**: ly account.

List your infographics
- **update_infographic**: Update an existing infographic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Easelly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my infographics in Easelly."

**🤖 AI Agent:**
> I've retrieved your infographics. You have 5 active designs, including 'Q1 Market Report' (ID: inf_123) and 'User Onboarding Flow'. Which one would you like to export or update?

---

**👤 You:**
> "Generate a PDF version for infographic 'inf_123'."

**🤖 AI Agent:**
> PDF generation triggered! I've successfully initiated the creation of the PDF for 'Q1 Market Report'. You can download the file here: [link]. Your document is now ready for distribution.

---

**👤 You:**
> "Export infographic ID 'inf_456' as a PNG image."

**🤖 AI Agent:**
> Image export complete! I've rendered 'User Onboarding Flow' as a high-quality PNG. You can access the direct link here: [link]. Would you like me to check the JSON structure of this design?


## ❓ FAQ

**Q: How do I find my Easelly API Key?**
Log in to your account and navigate to the settings or profile section to generate or copy your unique Pro API key.

**Q: What file formats are supported for export?**
You can export your infographics as PDF documents or high-quality JPG and PNG images using the respective generation tools.

**Q: Is an Easelly Pro account required?**
Yes, API access and advanced export features are exclusively available to Easelly Pro subscribers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/easelly](https://vinkius.com/mcp/easelly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Easelly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `easelly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Easelly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "easelly": {
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
