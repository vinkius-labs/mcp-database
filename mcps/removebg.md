# Remove.bg MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/removebg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/removebg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/removebg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Remove image backgrounds automatically in seconds using AI — process URLs or base64 images and manage your credit balance.

## Description
Integrate the world-class **Remove.bg** AI into your workflow to handle image processing tasks through natural language. This MCP server allows your AI agent to instantly strip backgrounds from photos, refine results, and monitor your API usage.

### What you can do

- **Background Removal** — Use the `remove_background` tool to process images via URL or base64. Customize output with parameters for size (HD, 4k), format (PNG, JPG, WebP), and subject type (person, product, car).
- **Result Improvement** — Enhance previously processed images using the `improve_result` tool to ensure the highest quality cutouts.
- **Account Management** — Monitor your API health and remaining credit balance with the `get_account` tool to avoid workflow interruptions.
- **Advanced Styling** — Add solid background colors, new background images, or shadows directly during the removal process.

### How it works

1. Subscribe to this server
2. Enter your Remove.bg API Key
3. Ask your AI to process images or check your balance from Claude, Cursor, or any MCP client

Perfect for e-commerce managers, designers, and developers who need to automate high-volume image editing without leaving their workspace.


## Available Tools
- **get_account**: bg account.

Get Remove.bg account info and credit balance
- **improve_result**: Improve a previously processed result
- **remove_background**: Returns the processed image as base64 data.

Remove the background from an image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Remove.bg** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my Remove.bg credit balance."

**🤖 AI Agent:**
> I've checked your account. You currently have 45.5 credits remaining and have used 5 credits in the current billing cycle.

---

**👤 You:**
> "Remove the background from this image URL: https://example.com/photo.jpg and return it as a PNG."

**🤖 AI Agent:**
> Processing image... I have successfully removed the background. You can download the processed PNG file from the link provided or I can show you the base64 data.

---

**👤 You:**
> "Improve the result for this image base64 string."

**🤖 AI Agent:**
> Applying improvement algorithms... The image has been refined for better edge quality and detail. Here is the updated result.


## Installation & Usage

To install and use the **Remove.bg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/removebg](https://vinkius.com/mcp/removebg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
