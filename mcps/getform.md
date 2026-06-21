# Getform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Automate form submissions and manage responses via Getform — submit data to endpoints and list submissions directly from your AI agent.

## Description
Connect your **Getform** account to any AI agent to streamline your data collection and form management workflows. This server allows you to interact with your form endpoints using natural language.

### What you can do

- **Form Submissions** — Programmatically submit data to any Getform endpoint using its unique Form ID. Perfect for automating lead capture or feedback loops.
- **Response Management** — Retrieve and list all submissions for a specific form to analyze entries without leaving your chat interface.
- **Data Integration** — Send structured JSON payloads including names, emails, and custom message blocks directly to your backend.

### How it works

1. Subscribe to this server
2. Enter your Getform API Key (found in your account settings)
3. Start submitting data or querying responses from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Test form endpoints and verify submissions directly from the code editor.
- **Marketers** — Quickly check for new leads or feedback entries from active campaigns.
- **Support Teams** — Automate the logging of customer inquiries into your form backend.


## Available Tools (2)
- **getform_list_submissions**: Requires Protected Mode (API Key).

List submissions for a specific form
- **getform_submit_form**: Supports standard fields and blocks like sender, email, text. This is a public endpoint.

Submit data to a specific Getform form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Getform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Submit a new contact request to form ID 'abc123xyz' with the name 'Alice' and email 'alice@example.com'."

**🤖 AI Agent:**
> I've successfully submitted the data to form abc123xyz. The submission has been recorded.

---

**👤 You:**
> "List the latest submissions for my Getform form 'form-id-789'."

**🤖 AI Agent:**
> I found 3 recent submissions for form 'form-id-789'. Here are the details: 1. From Bob (bob@...), 2. From Charlie (charlie@...), 3. From Diana (diana@...).

---

**👤 You:**
> "Send this JSON data to Getform endpoint 'xyz-999': { "feedback": "Great service!", "rating": 5 }."

**🤖 AI Agent:**
> The feedback data has been sent to the Getform endpoint 'xyz-999' successfully.


## ❓ FAQ

**Q: Do I need an API key to submit data to a form?**
The `submit_form` tool uses a public endpoint, so it only requires the Form ID. However, to list or view submissions using `list_submissions`, a valid API Key is required for security.

**Q: What format should the form data be in?**
You should provide a JSON object to the `data` parameter. For example: `{"name": "John Doe", "email": "john@example.com", "message": "Hello!"}`.

**Q: Can I see the content of the submissions directly in the AI chat?**
Yes! By using the `list_submissions` tool with your Form ID, the agent will retrieve and display the entries recorded for that specific form.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getform](https://vinkius.com/mcp/getform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Getform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `getform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Getform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "getform": {
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
