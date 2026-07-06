# FormKeep MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/formkeep)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage form submissions, automate backends, and oversee data retrieval via AI agents with FormKeep.

## Description
Connect your **FormKeep** account to any AI agent to automate your form data retrieval and submission management through the Model Context Protocol (MCP). FormKeep is the easiest way to add a backend to your HTML forms without writing a single line of server-side code. This MCP server enables you to retrieve submissions, manage your forms, and monitor incoming leads directly through natural conversation.

### Key Features

- **Submission Retrieval** — List all submissions for specific forms and fetch detailed data fields for individual records.
- **Spam Control** — Filter and manage spam submissions to ensure your data library stays clean and relevant.
- **Form Oversight** — Access and list all forms in your account, including their unique identifiers and setup metadata.
- **Data Management** — Delete specific submissions or clean up your records directly through simple AI commands.
- **Pagination Support** — Effortlessly navigate through large volumes of submission data with built-in pagination tools.
- **Real-time Monitoring** — Fetch recent submissions to keep your team informed of new inquiries or customer feedback.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your FormKeep API Token (found in your form's Reports tab)
3. Start managing your form data from Claude, Cursor, or any MCP client

### Who is this for?

- **Lead Generation Managers** — quickly check for new inbound inquiries or list recent leads for sales follow-up.
- **Frontend Developers** — verify form submissions and data integrity directly from your development environment.
- **Marketing Operations** — automate the retrieval of survey data and customer feedback for reporting and analysis.


## Available Tools (5)
- **get_form_details**: Get form metadata
- **get_submission**: Get submission details
- **list_forms**: List all forms
- **list_submissions**: List form submissions
- **delete_submission**: Remove a submission


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FormKeep** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 10 submissions for my 'Contact' form (ID: abc123)."

**🤖 AI Agent:**
> Retrieving submissions... I found the 10 most recent records for form abc123, including inquiries from 'Alice' and 'Bob'. Would you like to see the full data fields for any of them?

---

**👤 You:**
> "Show me all active forms in my FormKeep account."

**🤖 AI Agent:**
> Fetching forms... You have 3 active forms: 'Contact Us', 'Newsletter Signup', and 'Beta Feedback'. Which one would you like to inspect?

---

**👤 You:**
> "Delete submission ID '987654' from form 'abc123'."

**🤖 AI Agent:**
> Submission deleted! I've permanently removed the record from your FormKeep account. Your data library has been updated.


## ❓ FAQ

**Q: How do I get an API Token for FormKeep?**
You can find your secret API token in your FormKeep dashboard by navigating to the 'Reports' tab of your specific form.

**Q: Can I filter out spam submissions via the agent?**
Yes! The 'list_submissions' tool allows you to set the 'spam' parameter to false to exclude all entries flagged as spam by FormKeep.

**Q: Is it possible to delete individual submissions using the agent?**
Absolutely. Use the 'delete_submission' tool and provide the Form ID and Submission ID to permanently remove a record from your account.

**Q: How do I find my Form ID?**
The Form ID is the alphanumeric string found in your form's URL or under the 'Setup' tab in your FormKeep dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/formkeep](https://vinkius.com/mcp/formkeep)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FormKeep** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formkeep` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FormKeep** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formkeep": {
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
