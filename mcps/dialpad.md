# Dialpad MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dialpad)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Equip your AI agent to send office SMS, manage team contacts, and monitor call logs via the Dialpad API.

## Description
Integrate **Dialpad**, the AI-powered cloud communications platform, directly into your AI workflow. Manage your enterprise telephony, send and receive business SMS, track call logs and statistics, and update agent presence using natural language.

### What you can do

- **Messaging Control** — Send outbound business SMS to any E.164 formatted number directly from the chat.
- **Directory Management** — List team contacts and retrieve granular profile details for anyone in your organization.
- **Call Auditing** — Access real-time call logs and statistics to track answered, missed, or rejected rings.
- **Presence Management** — Update your availability status and custom markers to coordinate with your team effectively.

### How it works

1. Connect the Dialpad integration to your AI assistant.
2. Authorize using your Dialpad API Key (found in your admin settings).
3. Orchestrate your business communications and telephony through intuitive conversation.

### Who is this for?

- **Sales & Support Teams** — Send SMS and update status without leaving your primary workspace.
- **Operations Managers** — Audit call metrics and manage team directories via chat.
- **Office Admins** — Monitor organizational telephony usage and IVR structures instantly.


## Available Tools
- **upsert_business_contact**: Bootstrap an entirely mutable Contact array resolving Dialpad directories
- **wipe_directory_entry**: Irreversibly vaporize explicit contact constraints destroying Dialpad DB links
- **get_person_details**: Perform structural extraction of properties driving an explicit Extension
- **list_team_contacts**: 164 capacities directly.

Identify bounded routing spaces verifying explicit Business Directories
- **list_raw_call_logs**: Inspect deep internal arrays parsing real-time Telephony
- **get_agent_profile**: Enumerate explicitly attached structured rules traversing self-identities
- **list_call_statistics**: Retrieve explicit Cloud logging tracing rejected Call paths
- **list_ivr_departments**: Identify precise active arrays spanning IVR groupings
- **dispatch_office_sms**: 164.

Provision a massively scalable JSON Payload rendering outbound Business Texts
- **update_presence_status**: Mutate global Web boundaries substituting identifying Desktop status strings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dialpad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to '+1234567890' saying 'Your support ticket is resolved'."

**🤖 AI Agent:**
> I've successfully sent the SMS to +1234567890 via your Dialpad account. The message is now queued for delivery. Would you like me to track its status?

---

**👤 You:**
> "Show me the missed calls from this morning."

**🤖 AI Agent:**
> I've found 3 missed calls from this morning, including calls from '+1987654321' and '+15550123'. Would you like me to retrieve the contact details for these numbers?

---

**👤 You:**
> "Set my Dialpad status to 'In a meeting'."

**🤖 AI Agent:**
> Your Dialpad presence has been updated to 'In a meeting'. Your team members will now see this status on their dashboards. Should I set an expiration time for this status?


## ❓ FAQ

**Q: How do I get a Dialpad API Key?**
Log in to your Dialpad admin dashboard, navigate to **Admin Settings > My Company > Authentication > API Keys**, and generate a new key with the required scopes.

**Q: Can the agent receive SMS messages?**
This integration currently focuses on sending SMS and auditing logs. Incoming SMS can be monitored through the call and message logs in your account history.

**Q: Does it support international numbers?**
Yes, as long as your Dialpad account is configured for international calling/messaging, the agent can send SMS to any valid E.164 formatted number.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dialpad](https://vinkius.com/mcp/dialpad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dialpad** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dialpad` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dialpad** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dialpad": {
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
