# Formspree MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formspree)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage form submissions and automate data collection via Formspree — list entries, filter by date, and submit new data directly from your AI agent.

## Description
Connect your **Formspree** account to any AI agent to streamline your lead capture and form management workflows through natural conversation.

### What you can do

- **Submission Retrieval** — Fetch all entries for specific forms using their unique hash IDs to analyze leads or feedback.
- **Advanced Filtering** — Query submissions with pagination, date filters (`since`), and custom sort orders to find exactly what you need.
- **Direct Submission** — Programmatically submit data to forms including contact info, messages, and custom fields like company or phone.
- **Spam Management** — Optionally include or exclude flagged submissions in your queries to keep your data clean.

### How it works

1. Subscribe to this server
2. Enter your Formspree API Key
3. Start managing your form data from Claude, Cursor, or any MCP-compatible client

No more manual exporting of CSVs to check your latest leads. Your AI acts as a dedicated data analyst and form administrator.

### Who is this for?

- **Marketing Teams** — instantly retrieve latest campaign leads and filter by date without leaving the chat.
- **Developers** — test form submissions and verify data flow directly from the code editor.
- **Customer Support** — check recent form inquiries to respond to users faster and more efficiently.


## Available Tools (2)
- **submit_form**: Does not require API key authentication.

Submit data to a form
- **list_submissions**: Get submissions for a specific form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formspree** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 submissions for form hashid 'mqkvpogq'."

**🤖 AI Agent:**
> I've retrieved the 5 most recent submissions for form 'mqkvpogq'. They include entries from 'Alice Smith' and 'Bob Jones' regarding 'Project Inquiry'. Would you like to see the full message for any of these?

---

**👤 You:**
> "Check for any new submissions for form 'xknpdyzd' since 2024-01-01."

**🤖 AI Agent:**
> Searching for submissions since January 1st... I found 3 new entries. One is a newsletter signup and two are contact requests. Shall I summarize the contact requests for you?

---

**👤 You:**
> "Submit a test entry to form 'mqkvpogq' with name 'Test User' and message 'Hello from MCP'."

**🤖 AI Agent:**
> Submitting data... The test entry was successfully sent to form 'mqkvpogq'. Formspree confirmed the submission was received.


## ❓ FAQ

**Q: How can I see the most recent submissions for a specific form?**
Use the `list_submissions` tool with the form's `hashid`. You can set the `limit` parameter to control how many recent entries you want to retrieve.

**Q: Can I filter submissions to only show those received after a certain date?**
Yes! The `list_submissions` tool accepts a `since` parameter. Provide an ISO formatted date (e.g., 2023-12-01T00:00:00) to fetch only newer submissions.

**Q: Is it possible to test a form by sending data through the AI?**
Absolutely. Use the `submit_form` tool with the target `hashid`. You can provide details like `email`, `name`, and `message` to simulate a real user submission.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formspree](https://vinkius.com/mcp/formspree)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formspree** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formspree` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formspree** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formspree": {
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
