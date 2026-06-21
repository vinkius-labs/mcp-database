# Cloudmersive MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudmersive)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Validate data, scan files for viruses, and process documents with a suite of utility APIs for security and compliance.

## Description
Connect your **Cloudmersive** API account to any AI agent and simplify how you process documents, secure your web links, and manage media assets through natural conversation.

### What you can do

- **Security & Safety** — Scan any URL for viruses, malware, and phishing attempts in real-time to protect your ecosystem.
- **Document Conversion** — Convert any web page (URL) into a professional, high-fidelity PDF document via AI.
- **Image Manipulation** — Resize images from public URLs while preserving aspect ratio for web or social media use.
- **Email Intelligence** — Validate the authenticity and existence of email addresses to improve your outreach quality.
- **URL Insights** — Extract detailed metadata, headers, and status codes from any target website.
- **Operational Utility** — Manage your media and security workflows directly from Claude, Cursor, or any MCP client.

### How it works

1. Subscribe to this server
2. Enter your Cloudmersive API Key (found in your account dashboard)
3. Start processing your digital assets from your favorite AI assistant

### Who is this for?

- **Developers & DevOps** — quickly test document rendering and security scanning via simple AI commands.
- **Marketing & Content Teams** — automate image resizing and verify prospect emails directly from the workspace.
- **Security Analysts** — perform quick malware checks on suspicious links via the AI assistant.


## Available Tools (12)
- **analyze_text_sentiment**: Analyze text sentiment
- **check_cloudmersive_status**: Verify connectivity
- **convert_doc_to_pdf**: Convert document to PDF
- **convert_html_to_text**: Convert HTML to text
- **get_image_info**: Get image info
- **get_url_metadata**: Get URL metadata
- **resize_image**: Resize an image
- **scan_url**: Scan URL for threats
- **validate_domain**: Validate a domain
- **validate_email**: Validate an email
- **validate_phone**: Validate a phone number
- **validate_url**: Validate a URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloudmersive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the website 'https://example.com' is safe and has any viruses."

**🤖 AI Agent:**
> Scanning URL... The website 'https://example.com' is Clean. No viruses, malware, or phishing threats were detected by Cloudmersive. It is safe to visit.

---

**👤 You:**
> "Convert the page 'https://en.wikipedia.org/wiki/Artificial_intelligence' into a PDF."

**🤖 AI Agent:**
> PDF conversion initiated! I've rendered the Wikipedia page into a high-quality document. You can download your PDF here: [PDF URL].

---

**👤 You:**
> "Verify if the email 'john.doe@gmail.com' exists."

**🤖 AI Agent:**
> Verification complete! The email 'john.doe@gmail.com' is Valid. It has been confirmed as an active mailbox on the Gmail servers.


## ❓ FAQ

**Q: Can I scan a suspicious link for viruses via AI?**
Yes! Use the `scan_url_for_viruses` tool and provide the URL. Your agent will perform a real-time malware check and let you know if it's safe or malicious.

**Q: How do I convert a website to a PDF using the agent?**
Use the `convert_url_to_pdf` tool. Provide the target URL, and the agent will render the page and provide a link to the generated PDF document.

**Q: Is it possible to resize an image URL via AI?**
Absolutely. Use the `resize_image_from_url` action. Provide the image URL and the target width/height. The agent will return the resized image link.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudmersive](https://vinkius.com/mcp/cloudmersive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cloudmersive** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudmersive` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cloudmersive** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudmersive": {
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
