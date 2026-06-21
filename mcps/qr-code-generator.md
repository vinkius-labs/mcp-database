# QR Code Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qr-code-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate and decode QR codes for URLs, text, and data directly within your AI workflow.

## Description
Transform any text or URL into a high-quality QR code or decode existing ones using the **QR Code Generator** MCP server. This tool integrates the powerful goqr.me API to provide seamless image generation and data extraction.

### What you can do

- **Custom Generation** — Create QR codes with specific dimensions, colors, and background styles using the `create_qr_code` tool.
- **Data Decoding** — Extract information from existing QR codes by providing a public image URL to the `read_qr_code` tool.
- **Error Correction** — Adjust ECC levels (L, M, Q, H) to ensure your codes remain scannable even if partially damaged.
- **Format Flexibility** — Export your generated codes in various formats including PNG, SVG, JPEG, and EPS.
- **Styling Control** — Fine-tune margins, quiet zones, and character sets for localized data encoding.

### How it works

1. Subscribe to this server
2. No complex API keys are required for basic public usage
3. Start generating or reading QR codes directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Quickly generate QR codes for documentation, app deep links, or testing directly from the IDE.
- **Marketers** — Create branded QR codes with specific colors for campaigns without leaving the chat interface.
- **Operations Teams** — Decode QR codes from inventory photos or asset tags by simply pasting an image link.


## Available Tools
- **create_qr_code**: Generate a QR code image URL from data
- **read_qr_code**: Decode a QR code from an image URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QR Code Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a QR code for the URL https://vurb.io"

**🤖 AI Agent:**
> I've generated the QR code for you. You can view or download it here: [QR Code URL].

---

**👤 You:**
> "Generate a 400x400 blue QR code for the text 'Welcome to the Team' in PNG format."

**🤖 AI Agent:**
> The custom blue QR code (400x400) has been created. Here is your link: [QR Code URL].

---

**👤 You:**
> "Decode the QR code from this image: https://example.com/my-qr.png"

**🤖 AI Agent:**
> I've scanned the image. The QR code contains the following data: 'https://github.com/mcp-servers'.


## ❓ FAQ

**Q: Can I customize the color and size of the generated QR code?**
Yes! The `create_qr_code` tool allows you to specify the `size` (e.g., '300x300'), `color` (in RGB or Hex), and `bgcolor` to match your branding requirements.

**Q: How do I extract text from an existing QR code image?**
Use the `read_qr_code` tool and provide the `fileurl` of the image. The AI will decode the contents and return the stored text or URL to you instantly.

**Q: What is the 'ecc' parameter and which value should I use?**
ECC stands for Error Correction Code. It allows the QR code to be read even if it's dirty or damaged. Values range from 'L' (7% recovery) to 'H' (30% recovery). Use 'H' for codes that might face physical wear.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qr-code-generator](https://vinkius.com/mcp/qr-code-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QR Code Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `qr-code-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QR Code Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "qr-code-generator": {
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
