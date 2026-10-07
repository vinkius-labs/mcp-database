# Travel Document Timeline MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-document-timeline)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates a chronological schedule for travel preparations like passports and visas.

## Description
This MCP server builds a comprehensive due-date plan for all necessary travel preparations. By providing a travel date and required lead times, you can use `get_timeline_plan` to generate a step-by-step schedule for identity documents, logistics, health requirements, and more. It also includes tools like `validate_lead_time_config` to ensure your planning is complete and `calculate_readiness_score` to track your progress against deadlines.


## Available Tools (4)
- **get_category_summary**: Aggregates preparation tasks by category
- **calculate_readiness_score**: Determines how much of the preparation work is ahead of schedule
- **get_timeline_plan**: Generates a chronological schedule of all required travel preparations
- **validate_lead_time_config**: Ensures a provided set of lead times is logical and complete


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Document Timeline** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a travel timeline for a trip on 2025-06-01 with 30 days for identity and 14 days for logistics."

**🤖 AI Agent:**
> Your preparation schedule is ready. You should complete identity documents by 2025-05-02 and logistics by 2025-05-18.

---

**👤 You:**
> "Check if my lead times for identity and health are valid for a trip requiring both."

**🤖 AI Agent:**
> The lead time configuration is valid and covers all mandatory categories.

---

**👤 You:**
> "What is the summary of tasks for the health category in my timeline?"

**🤖 AI Agent:**
> The health category contains 2 tasks, with the earliest deadline on 2025-04-15 and the latest on 2025-05-10.


## ❓ FAQ

**Q: How do I generate a preparation schedule?**
You can use the `get_timeline_plan` tool by providing your intended travel date and the required lead times for each category.

**Q: Can I add a safety margin to my deadlines?**
Yes, the `get_timeline_plan` tool accepts an optional `bufferDays` parameter to add extra days to every lead time.

**Q: How can I check if my travel planning is on track?**
Use the `calculate_readiness_score` tool with your generated timeline and the current date to see how many deadlines have passed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-document-timeline](https://vinkius.com/en/ai-agent-connect/travel-document-timeline)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Document Timeline** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-document-timeline` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Document Timeline** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-document-timeline": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
