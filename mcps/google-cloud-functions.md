# Google Cloud Functions MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-cloud-functions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it invokes a single Google Cloud Function. That's its only function, and nothing else. Incredible for letting your AI execute secure serverless compute.

## Description
This server strips away dangerous global GCP permissions. It gives your AI agent one surgical superpower: **the ability to synchronously invoke one specific Cloud Function and read its response.**

By strictly scoping access, your AI can safely offload complex math, heavy data processing, or internal API calls to a dedicated serverless function without having permission to execute arbitrary code across your account.

### The Superpowers

- **Absolute Containment:** The agent is locked to a single function endpoint. It cannot invoke other functions or modify source code.
- **Synchronous Compute:** The agent waits for the compute payload to finish, allowing it to seamlessly continue its thought process.
- **Plug & Play Processing:** Instantly gives your agent access to your proprietary enterprise logic isolated inside a serverless container.


## Available Tools
- **gcf_invoke_function**: Use this to execute remote business logic or heavy processing tasks.

Invoke the configured Google Cloud Function


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Cloud Functions** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Invoke the function to resize this image."

**🤖 AI Agent:**
> I've invoked the function. The response returned a new URL for the resized image.

---

**👤 You:**
> "Call the scraper function with the URL 'https://example.com' as payload."

**🤖 AI Agent:**
> The function executed successfully. The result object contains the extracted text from the page.

---

**👤 You:**
> "Run the heavy calculation and pass {"dataset_id": "12345"}."

**🤖 AI Agent:**
> The invocation failed with a 'timeout' error. We may need to optimize the payload or function timeout settings.


## ❓ FAQ

**Q: Why limit the agent to a single Cloud Function?**
To enforce zero-trust security. An autonomous AI agent should not have the ability to execute arbitrary serverless functions (like wiping a database or sending mass emails) across your cloud infrastructure.

**Q: How are responses handled?**
The MCP will automatically parse valid JSON responses returned by the Cloud Function. If the function returns an error or a timeout, the execution ID and the specific error string will be returned to the agent.

**Q: Can it invoke Gen 2 Cloud Functions?**
Yes! The tool uses the standard Google Cloud Functions REST API (`:call` endpoint), which is compatible with both 1st gen and 2nd gen functions, provided the IAM Service Account has the `roles/cloudfunctions.invoker` permission.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-cloud-functions](https://vinkius.com/mcp/google-cloud-functions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Cloud Functions** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-cloud-functions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Cloud Functions** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-cloud-functions": {
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
