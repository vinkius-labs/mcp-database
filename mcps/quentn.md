# Quentn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quentn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build email marketing funnels with visual automation workflows designed for German-speaking markets and GDPR compliance.

## Description
Connect your **Quentn** account to any AI agent and take full control of your CRM orchestration and marketing automation through natural conversation. Quentn provides a powerful platform for managing customer relationships and complex marketing sequences, and this integration allows you to retrieve contact metadata, trigger campaign sequences, and manage tags (terms) directly from your chat interface.

### What you can do

- **Contact & CRM Orchestration** — List, create, and update contacts with detailed profile metadata programmatically to ensure your sales database is always synchronized.
- **Campaign Lifecycle Management** — Access and monitor your marketing campaigns and trigger specific sequences for contacts directly from the AI interface.
- **Tag & Segment Control** — Manage terms (tags) to maintain a clear overview of your audience segmentation via natural language.
- **Omnichannel Communication** — Send automated emails through the Quentn system to ensure consistent customer engagement.
- **Operational Monitoring** — Track system activity and manage custom fields to ensure your marketing stack is always optimized using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Quentn API Key and unique Base URL from your API Info settings
3. Start managing your CRM and campaigns from Claude, Cursor, or any MCP-compatible client

No more manual contact entry or searching through sequences. Your AI acts as a dedicated marketing automation manager or CRM coordinator.

### Who is this for?

- **Marketing Managers** — quickly retrieve campaign statuses and monitor segment growth without switching apps.
- **Sales Teams** — automate the management of lead records and track interaction history via natural conversation.
- **Operations Teams** — streamline the retrieval of contact metadata and monitor organizational health directly within the chat.


## Available Tools
- **create_contact**: Create a new contact
- **delete_contact**: Delete a contact
- **get_campaign**: Get campaign details
- **get_contact**: Get contact details by ID
- **get_tag_details**: Get details for a specific tag
- **list_campaigns**: List all campaigns
- **list_contacts**: List all contacts
- **list_tags**: List all tags/terms
- **list_users**: List system users
- **send_email**: Send an email to a contact
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quentn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts tagged as 'VIP' in Quentn."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 12 active profiles tagged as 'VIP', including 'Alice Brown' and 'Acme Corp'. Would you like to check the engagement for any of them?

---

**👤 You:**
> "Show me all contacts who opened my last email campaign but did not click any link."

**🤖 AI Agent:**
> 234 contacts opened the "May Product Update" campaign but did not click. Open rate: 42% (234 of 557 recipients). Click rate for these openers: 0%. Top segments: "Trial Users" (89 contacts), "Inactive 30 days" (67), "Newsletter Only" (48). Average time spent on email: 4.2 seconds (suggests scanning, not reading). Recommendation: A/B test subject lines and move CTAs above the fold for this cohort. 12 contacts are tagged as "High Value" and may benefit from personalized follow-ups.

---

**👤 You:**
> "Create a new contact with tag VIP Customer and add them to the onboarding automation sequence."

**🤖 AI Agent:**
> Contact created successfully. Name: Alexandra Petrov. Email: a.petrov@scaleup.io. Tag: VIP Customer applied. Added to automation: "VIP Onboarding Sequence" (5 emails over 14 days). First email "Welcome to VIP" scheduled to send in 15 minutes. The contact has been assigned to your CRM with lead score: 85/100. Custom fields populated: Company: ScaleUp Inc, Role: Head of Product, Source: Partner Referral.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific contact just by providing their ID?**
Yes! Use the `get_contact` tool. Your agent will respond with complete metadata, including tags, custom fields, and engagement history in seconds.

**Q: Where do I find my Quentn Base URL?**
Log in to Quentn, go to **My Account** > **API Info**. Your unique base URL follows the pattern `https://<system_id>.<server_id>.quentn.com/public/api/V1`.

**Q: How do I add a tag to a contact?**
Use the `update_contact` tool and include the new tag in the 'terms' field of the request body.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quentn](https://vinkius.com/mcp/quentn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quentn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `quentn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quentn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quentn": {
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
