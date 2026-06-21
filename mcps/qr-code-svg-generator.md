# QR Code SVG Generator MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/qr-code-svg-generator)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/qr-code-svg-generator-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/qr-code-svg-generator-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate vector SVG QR Codes completely local. Prevent data leakage of sensitive Pix keys or JWT tokens to public API generators.

## Description
AI Agents that generate PDF contracts, event tickets, or Pix billing codes often need to embed a QR Code. Since LLMs cannot render images, they usually send the sensitive payload (like a payment key) to a public API like `api.qrserver.com`. This is a massive security and privacy breach. This MCP solves that by generating the QR Code locally.

### The Superpowers

- **Zero Data Leakage:** Generates the QR Code mathematically inside the V8 engine without any network requests.
- **Vector Scalability:** Returns an SVG string that can be safely embedded into HTML emails, PDFs, or React components.


## Available Tools
- **generate_qr**: Pass the content string and receive a complete SVG markup ready for embedding in HTML or saving.

Generates vector SVG QR Codes instantly offline. Prevents data leakage of sensitive Pix keys or tokens to public API generators


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QR Code SVG Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a QR Code for this event ticket URL: `https://vinkius.com/ticket/123`"

**🤖 AI Agent:**
> Generated QR Code SVG: Output returned successfully.

---

**👤 You:**
> "Create a QR Code for this PIX payment payload so I can embed it in the invoice."

**🤖 AI Agent:**
> Generated QR Code SVG: Output returned successfully.

---

**👤 You:**
> "I need an SVG QR code containing this secure WiFi password configuration."

**🤖 AI Agent:**
> Generated QR Code SVG: Output returned successfully.


## Installation & Usage

To install and use the **QR Code SVG Generator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qr-code-svg-generator](https://vinkius.com/mcp/qr-code-svg-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
