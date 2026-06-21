# QR Code SVG Generator MCP Server

Generate vector SVG QR Codes completely local. Prevent data leakage of sensitive Pix keys or JWT tokens to public API generators.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/qr-code-svg-generator)

## Overview
**Category:** productivity
**Tools Count:** 1

## Description
AI Agents that generate PDF contracts, event tickets, or Pix billing codes often need to embed a QR Code. Since LLMs cannot render images, they usually send the sensitive payload (like a payment key) to a public API like `api.qrserver.com`. This is a massive security and privacy breach. This MCP solves that by generating the QR Code locally.

### The Superpowers

- **Zero Data Leakage:** Generates the QR Code mathematically inside the V8 engine without any network requests.
- **Vector Scalability:** Returns an SVG string that can be safely embedded into HTML emails, PDFs, or React components.


## Available Tools
- **generate_qr**: Pass the content string and receive a complete SVG markup ready for embedding in HTML or saving.

Generates vector SVG QR Codes instantly offline. Prevents data leakage of sensitive Pix keys or tokens to public API generators


## Installation & Usage

To install and use the **QR Code SVG Generator** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/qr-code-svg-generator](https://vinkius.com/mcp/qr-code-svg-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
