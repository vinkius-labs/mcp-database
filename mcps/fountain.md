# Fountain MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fountain)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Automate high-volume hiring, manage applicant funnels, and track hiring goals via AI agents with Fountain.

## Description
Connect your **Fountain** account to any AI agent to automate your high-volume hiring and applicant lifecycle management through the Model Context Protocol (MCP). Fountain is designed specifically for frontline workforce management, allowing you to streamline every stage from sourcing to onboarding. This MCP server enables you to manage your applicant funnels, track hiring progress, and oversee worker profiles directly through natural conversation.

### Key Features

- **Applicant Oversight** — List all applicants, search by email or funnel, and fetch detailed profiles including transition history.
- **Funnel & Stage Management** — Access and list your hiring funnels and specific stages to understand your pipeline health.
- **Hiring Goal Tracking** — Monitor your progress against specific hiring targets and performance metrics.
- **Opening Management** — List all active job openings and fetch detailed metadata for specific positions.
- **Interview Coordination** — List and oversee scheduled interview sessions across your organization.
- **Worker Profiles** — Access metadata for individuals who have successfully completed the hiring process.
- **Sourcing Insights** — Monitor published job posts across various channels to optimize your recruitment reach.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fountain API Token (found in Company Settings > Developer Settings)
3. Start managing your frontline recruitment directly from your AI agent


## Available Tools (12)
- **list_applicant_notes**: Get applicant discussion
- **list_applicants**: List job applicants
- **list_funnels**: List hiring funnels
- **list_hiring_goals**: List hiring targets
- **list_interview_sessions**: List scheduled interviews
- **list_job_posts**: List published job posts
- **list_funnel_stages**: List stages in a funnel
- **list_workers**: List hired workers
- **get_account_details**: Get organization attributes
- **get_applicant**: Get applicant details
- **get_opening_details**: Get opening metadata
- **list_openings**: List active job openings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fountain** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job openings in Fountain."

**🤖 AI Agent:**
> Retrieving openings... I found 5 active job positions, including 'Delivery Driver' and 'Warehouse Associate'. Would you like to see the details for any of these?

---

**👤 You:**
> "Show me the last 10 applicants for the 'Delivery' funnel."

**🤖 AI Agent:**
> Fetching applicants... I found 10 recent submissions for the 'Delivery' funnel. 3 are currently in the 'Interview' stage and 2 are in 'Background Check'.

---

**👤 You:**
> "Get the hiring goals summary for this quarter."

**🤖 AI Agent:**
> Retrieving goals... You are currently at 75% of your 'Warehouse Hiring' goal and 90% of your 'Customer Support' target for this quarter.


## ❓ FAQ

**Q: How do I get an API Token for Fountain?**
You can find or generate your API token in your Fountain dashboard under Company Settings > Developer Settings.

**Q: Does Fountain support bulk actions?**
Yes, the Fountain API is designed for scale. While this MCP server focuses on management and retrieval, bulk advance and transitions are supported by the core platform.

**Q: Can I see interview schedules via the agent?**
Yes, the 'list_interview_sessions' tool allows you to retrieve all scheduled and past interview sessions directly from your account.

**Q: Is worker data accessible after hire?**
Yes, you can use the 'list_workers' tool to access profiles of individuals who have successfully transitioned to 'hired' status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fountain](https://vinkius.com/mcp/fountain)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fountain** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fountain` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fountain** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fountain": {
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
