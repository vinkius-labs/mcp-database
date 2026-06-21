# MJML (Email Markup) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mjml-email-markup)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mjml-email-markup-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mjml-email-markup-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Transpile MJML markup into responsive, high-quality HTML emails directly from your AI agent.

## Description
Connect the **MJML** engine to your AI agent to generate professional, responsive email templates using natural language. MJML is the industry standard for ensuring emails look great across all clients like Outlook, Gmail, and Apple Mail.

### What you can do

- **Responsive Rendering** — Convert MJML XML or JSON strings into production-ready HTML in seconds
- **Email Prototyping** — Rapidly iterate on email designs within your chat or code editor
- **Best Practices** — Ensure your markup follows email client standards automatically without manual table hacking

### How it works

1. Subscribe to this server
2. Enter your MJML Application ID and API Key
3. Start rendering email markup from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Generate email HTML without leaving the IDE or dealing with complex CSS inlining
- **Marketing Teams** — Quickly preview how MJML-based campaigns will look before deployment
- **Designers** — Validate MJML syntax and see immediate visual results through the AI presenter


## Available Tools
- **render_mjml**: Provide the raw MJML XML or JSON string.

Render MJML markup to responsive HTML


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MJML (Email Markup)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Render this MJML code to HTML: <mjml><mj-body><mj-section><mj-column><mj-text>Hello World</mj-text></mj-column></mj-section></mj-body></mjml>"

**🤖 AI Agent:**
> I've processed your MJML markup. The transpiled responsive HTML is ready and follows all email client best practices. You can view the output in the presenter below.

---

**👤 You:**
> "Can you use render_mjml to convert a JSON-based MJML structure into a responsive email?"

**🤖 AI Agent:**
> Absolutely. Please provide the MJML JSON string, and I will use the `render_mjml` action to generate the corresponding high-quality HTML for you.

---

**👤 You:**
> "Generate a responsive button in MJML and render it to HTML."

**🤖 AI Agent:**
> I've created a responsive button using `<mj-button>`. I am now running `render_mjml` to provide you with the production-ready HTML code and a visual preview.


## Installation & Usage

To install and use the **MJML (Email Markup)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mjml-email-markup](https://vinkius.com/mcp/mjml-email-markup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
