# Viesus MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/viesus)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enhance photos automatically with AI that adjusts exposure, color balance, and sharpness to make every image look professional.

## Description
Connect your **Viesus** account to any AI agent and simplify your professional image processing and enhancement workflows through natural conversation.

### What you can do

- **AI Enhancement** — Apply powerful upscaling, face restoration, and automatic color correction to your photos.
- **Job Monitoring** — Upload images and track the real-time status of your enhancement requests (queued, processing, completed).
- **Content Retrieval** — Fetch direct download links for your processed images and retrieve technical metadata like resolution and color space.
- **Account Management** — Monitor your credit balance and view the history of all processing jobs.
- **Preset Library** — List and select from predefined enhancement configurations optimized for different photo types.

### How it works

1. Subscribe to this server
2. Enter your Viesus Cloud API Access Token
3. Start enhancing your visual content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Professional Photographers** — quickly upscale low-res images and apply color correction via simple AI commands.
- **Content Creators** — automate the retouching of social media assets and verify processing history.
- **E-commerce Teams** — ensure product photos meet technical standards by retrieving metadata and applying consistent presets.


## Available Tools
- **check_api_health**: Verify Viesus API status
- **enhance_image_ai**: Apply AI enhancement to an image
- **get_account_credit_balance**: Check remaining API credits
- **get_enhanced_image_url**: Retrieve the final image download link
- **get_image_metadata**: Retrieve technical metadata for an image
- **get_enhancement_job_status**: Check the status of an enhancement job
- **get_api_version_info**: Retrieve API version details
- **list_supported_file_formats**: List supported image formats
- **list_processing_history**: List recent image processing jobs
- **list_enhancement_presets**: List available enhancement configurations
- **list_configured_webhooks**: List active webhooks
- **upload_image_to_viesus**: Upload an image for processing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Viesus** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my Viesus credit balance."

**🤖 AI Agent:**
> I've retrieved your balance. You currently have 450 credits available for image processing. Would you like to check the status of your last enhancement job?

---

**👤 You:**
> "Enhance image 'img_12903' using the 'standard-high' preset."

**🤖 AI Agent:**
> AI enhancement initiated! The job has been queued with ID job_8823. I'll monitor the status and let you know as soon as the enhanced version is ready for download.

---

**👤 You:**
> "Show me the technical metadata for the image I just uploaded."

**🤖 AI Agent:**
> Fetching metadata... The image (ID: img_10293) has a resolution of 4000x3000px, uses the sRGB color space, and is in JPEG format. Shall we apply an enhancement preset to it?


## ❓ FAQ

**Q: Can I check how many credits I have left in Viesus?**
Yes! Use the `get_account_credit_balance` tool. Your agent will retrieve the current number of processing credits available in your account.

**Q: How do I download the enhanced version of my image?**
Once the job status is 'completed', use the `get_enhanced_image_url` tool with your Job ID to get the direct download link for the final photo.

**Q: What are the supported file formats for enhancement?**
You can run the `list_supported_file_formats` query to see a complete and up-to-date list of all input and output formats supported by the Viesus API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/viesus](https://vinkius.com/mcp/viesus)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Viesus** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `viesus` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Viesus** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "viesus": {
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
