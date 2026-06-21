# Gainsight CS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gainsight-cs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer success, track health scores, and oversee the timeline via AI agents with Gainsight CS.

## Description
Connect your **Gainsight Customer Success** (NXT) instance to any AI agent to automate your customer retention and engagement operations through the Model Context Protocol (MCP). Gainsight is the industry-standard platform for customer success, empowering CSMs to manage health scores, track activities, and close CTAs. This MCP server enables you to retrieve company metadata, log timeline events, and oversee cockpit tasks directly through natural conversation.

### Key Features

- **Company Health Oversight** — List all customer companies, retrieve detailed profiles including health scores, and verify CSM assignments instantly.
- **Timeline Activity Management** — Access the customer activity timeline and programmatically log new calls, meetings, or notes directly from your chat interface.
- **People & Contact Data** — Access detailed profile information for customers and partners managed within the Gainsight People object.
- **Cockpit Automation** — List and manage Calls to Action (CTAs) and associated tasks to stay on top of your retention playbook.
- **Workforce Insights** — Verify your own identity and profile details to ensure you are working in the correct account context.
- **Real-time Synchronization** — Keep your customer success strategy accessible to your AI assistant without leaving your primary workspace.
- **NXT API Integration** — Leverage the power of the Gainsight NXT platform with secure header-based authentication.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gainsight Domain and Access Key (found in Administration > Connectors 2.0 > Gainsight API)
3. Start managing your customer success data from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers** — quickly check an account's health score or log a quick meeting note without navigating the dashboard.
- **CS Operations** — automate the retrieval of CTA metadata or verify company mappings via simple AI commands.
- **Account Executives** — get a real-time overview of customer interaction history before renewal or expansion discussions.


## Available Tools (12)
- **verify_api_connection**: Verify connection
- **log_timeline_activity**: Log new activity
- **get_cta_metadata**: Get CTA details
- **get_company_health**: Get company metadata
- **get_my_identity**: Get current user profile
- **get_person_details**: Get person metadata
- **get_task_metadata**: Get task details
- **list_calls_to_action**: List cockpit CTAs
- **list_customer_companies**: List Gainsight companies
- **list_crm_people**: List Gainsight people
- **list_cockpit_tasks**: List cockpit tasks
- **list_timeline_events**: List timeline activities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gainsight CS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my top 5 customer companies and their health scores."

**🤖 AI Agent:**
> Retrieving companies... I found your top customers, including 'Acme Corp' (Health: 85/Green) and 'Globex' (Health: 42/Red). Would you like to see the pending CTAs for Globex?

---

**👤 You:**
> "Log a 'Call' activity for 'Acme Corp' (ID: 12345) saying 'Discussed Q4 renewal'."

**🤖 AI Agent:**
> Activity logged! I have successfully added the 'Discussed Q4 renewal' entry to the Acme Corp timeline. It is now visible to the entire team.

---

**👤 You:**
> "Show me all pending CTAs in my Gainsight cockpit."

**🤖 AI Agent:**
> Fetching cockpit... I found 4 pending CTAs, including 'Risk: Low Adoption' for Stark Industries and 'Expansion: Add Seats' for Wayne Enterprises.


## ❓ FAQ

**Q: How do I get an Access Key for Gainsight?**
Log in to your Gainsight NXT instance, navigate to Administration > Connectors 2.0 > Gainsight API, and generate a new Access Key.

**Q: What is the 'Domain' required for setup?**
Your domain is the base URL of your cloud instance (e.g., 'acme.gainsightcloud.com'). Do not include 'https://' or any path prefixes.

**Q: Can I log activity directly to the customer timeline?**
Yes! Use the 'log_timeline_activity' tool. Provide the subject, note, and the associated Company ID to instantly add an entry to their timeline.

**Q: Are health scores accessible via the agent?**
Yes, when you use 'get_company_health', the agent retrieves the current health score metadata along with the assigned CSM and other attributes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gainsight-cs](https://vinkius.com/mcp/gainsight-cs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gainsight CS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gainsight-cs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gainsight CS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gainsight-cs": {
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
