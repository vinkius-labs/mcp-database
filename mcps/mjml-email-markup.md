# MJML (Email Markup) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mjml-email-markup)
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


## Available Tools (1)
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


## ❓ FAQ

**Q: Can I render MJML from a JSON string instead of XML?**
Yes! The `render_mjml` tool accepts both raw MJML XML and MJML JSON strings. The engine will automatically detect the format and transpile it into responsive HTML.

**Q: What is the maximum size of the generated HTML output?**
The integration supports an egress limit of up to 5MB, which is more than enough for even the most complex and content-heavy responsive email templates.

**Q: Does the tool validate my MJML syntax during rendering?**
Yes, the `render_mjml` tool uses the official MJML engine which performs validation during the transpilation process to ensure the resulting HTML is compliant with email client best practices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mjml-email-markup](https://vinkius.com/mcp/mjml-email-markup)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MJML (Email Markup)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mjml-email-markup` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MJML (Email Markup)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mjml-email-markup": {
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
