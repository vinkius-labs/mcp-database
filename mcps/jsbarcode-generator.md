# JSBarcode Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jsbarcode-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Generate mathematically exact 1D barcodes (Code128, EAN-13, UPC, ITF, Codabar) as pure SVG vectors for shipping labels and inventory.

## Description
When an AI Agent in logistics needs to generate a scannable barcode for a shipping label, it absolutely cannot hallucinate the bar patterns — one wrong stripe and the scanner fails. This MCP uses JSBarcode (1.2M+ weekly downloads) to generate mathematically perfect barcodes.

### The Superpowers

- **20+ Formats:** CODE128, EAN13, EAN8, UPC, CODE39, ITF14, Codabar, pharmacode, and more.
- **Pure SVG:** No native image dependencies. Returns clean SVG markup embeddable in any HTML.


## Available Tools (1)
- **generate_barcode**: Pass the text to encode and the format (CODE128, EAN13, UPC, CODE39, ITF14, etc.). The engine returns valid SVG markup that can be embedded directly in HTML or printed. Never attempt to draw barcode patterns yourself.

Generates mathematically exact 1D barcodes (Code128, EAN-13, UPC, ITF, Codabar) as pure SVG vectors for shipping labels, inventory tags, and retail products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JSBarcode Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a Code128 barcode for SKU 'ABC-12345'."

**🤖 AI Agent:**
> Barcode Generated: SVG with 2,340 bytes.

---

**👤 You:**
> "Create an EAN-13 barcode for product number 5901234123457."

**🤖 AI Agent:**
> Barcode Generated: Valid EAN-13 SVG.


## ❓ FAQ

**Q: What barcode formats are supported?**
CODE128 (A/B/C), EAN13, EAN8, EAN5, EAN2, UPC, UPCE, CODE39, ITF, ITF14, MSI (10/11/1010/1110), pharmacode, and codabar.

**Q: Does it require canvas or native image libraries?**
No. It uses @xmldom/xmldom for pure XML-based SVG generation — zero native dependencies, fully Edge-compatible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jsbarcode-generator](https://vinkius.com/mcp/jsbarcode-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JSBarcode Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jsbarcode-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JSBarcode Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jsbarcode-generator": {
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
