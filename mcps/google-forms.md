# Google Forms MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-forms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Analyze datasets actively — list active Google Forms, query exact responses, and fetch metadata programmatically.

## Description
Connect your **Google Forms** infrastructure to a conversational AI assistant. You will bypass the need to constantly refresh CSV downloads or read through dense graphical charts by chatting directly with the pipeline stream.

### What you can do

- **Forms Aggregation** — List available forms by file ID to pinpoint exact surveys you are running over your customer base
- **Rapid Metadata Validation** — Inspect the schema of each active form directly to verify exactly what questions your marketing team is querying
- **Live Response Streaming** — Pull raw answering data and aggregated insights of all recent form submits right inside your chat environment seamlessly

### How it works

1. Install and subscribe to the server hook
2. Authorize via standard OAuth 2.0 mechanisms pointing to Workspace
3. Execute advanced read commands querying from your form matrix

### Who is this for?

- **Marketers & Analysts** — run quick summarization on customer NPS score trends without diving into raw CSV grids daily
- **Event Coordinators** — retrieve exact answers and confirmations from attendees using targeted IDs over text


## Available Tools (2)
- **get_form_metadata**: Get metadata and structure of a Google Form
- **get_form_responses**: Get all responses for a Google Form


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Forms** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read the form metadata and structure for the Form ID 'abc123xyz'."

**🤖 AI Agent:**
> I've fetched the structure. The active Form is titled 'Post-Event Feedback 2024'. It contains 4 explicit questions, including 'Rate your experience (1-10)' and 'Freeform Comments'.

---

**👤 You:**
> "Fetch the responses recorded today in the Sales Survey (Form ID abc). Summarize the general satisfaction."

**🤖 AI Agent:**
> I've captured 22 recent responses. Across those payloads, the prevalent satisfaction score hovers between 8 and 9. Top positive highlight: 'Fast customer service'. Negative outliers point out a lack of documentation.

---

**👤 You:**
> "List all active form instances under my account to find the latest specific quiz run."

**🤖 AI Agent:**
> Search initialized. Under your root index I discovered two forms matching normal schemas: 'Marketing Q1 Trends' (ID 4122) and 'Staff Quiz Baseline' (ID 198a). Which one should I focus on?


## ❓ FAQ

**Q: Can this server physically create a new Google Form from scratch using instructions?**
No. Google Forms API capabilities prioritize analytical reading of existing surveys (pull responses, list metadata). Destructive changes or creation matrices are not optimized here.

**Q: Do I need any specific permission boundaries on Google SDKs to extract data?**
You strictly need the 'googleapis.com/auth/forms.responses.readonly' and 'forms.body.readonly' scopes toggled via cloud. The system operates purely in minimal ReadOnly mode.

**Q: Is pagination natively supported when I pull thousands of responses?**
Yes. Due to Vurb core Egress controls, any call against a hyper-populated response matrix will logically paginate into manageable blocks ensuring stability across agents without truncating context loss.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-forms](https://vinkius.com/mcp/google-forms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Forms** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-forms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Forms** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-forms": {
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
