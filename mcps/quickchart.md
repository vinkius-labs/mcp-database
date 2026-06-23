# QuickChart MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quickchart)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Automate data visualization via QuickChart — generate charts, QR codes, barcodes, and word clouds directly from any AI agent.

## Description
Connect **QuickChart** to your AI agent to transform raw data into professional visuals instantly. This server provides a comprehensive suite of tools for generating static images of charts, codes, and text visualizations.

### What you can do

- **Chart.js Rendering** — Generate high-quality Chart.js images (v2, v3, or v4) from JSON configurations using `get_chart_url` or `render_chart_post`.
- **QR Codes & Barcodes** — Create customized QR codes with logos and various barcode formats (UPC, EAN, Code128) using `get_qr_url` and `get_barcode_url`.
- **Word Clouds** — Transform text blocks into beautiful word cloud images with custom fonts and colors via `get_wordcloud_url`.
- **Short URLs** — Generate permanent, shareable links for your visualizations with `create_chart_short_url`.
- **Complex Rendering** — Handle large datasets and complex configurations using POST requests to avoid URL length limits.

### How it works

1. Subscribe to this server
2. (Optional) Enter your QuickChart API Key for higher rate limits
3. Start generating visuals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly visualize trends and distributions without leaving the chat interface
- **Developers** — generate barcodes or QR codes for documentation or testing on the fly
- **Marketers** — create word clouds from customer feedback or social media text for reports


## Available Tools (9)
- **create_chart_short_url**: js configuration.

Generate a permanent short URL for a chart
- **get_barcode_url**: Construct a GET URL for a barcode image
- **get_chart_url**: Best for simple charts.

Construct a GET URL for a chart image
- **get_graphviz_url**: Construct a GET URL for a GraphViz diagram
- **get_qr_url**: Construct a GET URL for a QR code image
- **get_wordcloud_url**: Construct a GET URL for a word cloud image
- **render_apex_chart**: Render an Apex Chart and return as base64 data URI
- **render_chart_post**: js configurations that exceed URL length limits.

Render a complex chart and return as base64 data URI
- **render_google_chart**: Render a Google Chart and return as base64 data URI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QuickChart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a bar chart showing sales: Jan (100), Feb (150), Mar (120)."

**🤖 AI Agent:**
> I've generated the chart for you. You can view the bar chart showing the sales trend for the first quarter here: [Chart URL]

---

**👤 You:**
> "Create a QR code for 'https://vurb.com' with a rounded dot style."

**🤖 AI Agent:**
> I've created your customized QR code. Here is the link to the image: [QR Code URL]

---

**👤 You:**
> "Generate a word cloud from this text: 'AI automation efficiency productivity growth innovation'."

**🤖 AI Agent:**
> I've processed the text and generated a word cloud visualization for you: [Word Cloud URL]


## ❓ FAQ

**Q: What should I do if my chart configuration is too large for a standard URL?**
You should use the `render_chart_post` tool. It sends the configuration via a POST request, which supports much larger datasets and complex Chart.js objects that would otherwise exceed URL length limits.

**Q: Can I add a logo to the center of a QR code?**
Yes! When using the `get_qr_url` tool, you can provide a URL in the `centerImageUrl` parameter to overlay an image or logo in the middle of your generated QR code.

**Q: How can I get a permanent link for a chart to share with others?**
Use the `create_chart_short_url` tool. It generates a permanent, short URL hosted by QuickChart that you can easily share in documents or messages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickchart](https://vinkius.com/mcp/quickchart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QuickChart** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `quickchart` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QuickChart** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quickchart": {
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
