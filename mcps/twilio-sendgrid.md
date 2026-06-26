# Twilio SendGrid MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twilio-sendgrid)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Equip your AI agent with capabilities to natively dispatch HTML emails, prune suppression bounce lists, and manage marketing contacts via the SendGrid API.

## Description
Unleash your AI agent over **Twilio SendGrid's** trusted enterprise email platform. Transform your chat interface into a fully-fledged communications command center. By implementing this MCP server, your LLM gains the power to investigate unaddressed hard bounces, dispatch highly contextual custom emails, and automatically organize sprawling marketing directories.

### What you can do

- **Live Email Dispatching** — Dictate a tailored email to your agent and order it to use `dispatch_email` to send fully authenticated outbound HTML campaigns
- **Bounces & Suppression Auditing** — Ask the AI to identify why recent deliveries failed using `list_bounces` and tell it to permanently pardon specific addresses via `delete_bounce`
- **Dynamic Template Inspection** — Fetch all your stored transaction shells (`list_dynamic_templates`) and inspect precise structure iterations to verify UI before broadcasting
- **CRM Growth Automation** — Continuously append or enrich subscriber details straight from conversational prompts by executing `create_marketing_contact` on the fly

### How it works

1. Enable the targeted server component inside your client environment
2. Supply your encrypted `SendGrid API Key` bearing adequate sub-user permissions
3. Engage Cursor or Claude organically to query unsubscriptions or force send notifications immediately

### Who is this for?

- **Customer Success Managers** — organically instruct your AI to search for an angry customer's email across 'bounces', 'spam', or 'unsubscribes' to verify deliverability
- **Software Devs** — test specific edge-cases of dynamic templates bypassing Postman UI just by asking Claude to shoot a trial template straight to your inbox
- **Marketing Integrators** — query the global subscriber list numbers daily alongside other metrics completely through chat


## Available Tools (16)
- **list_single_sends**: List all marketing single-send campaigns
- **delete_bounce**: This action is destructive on the suppression record.

Removes an email from the bounce suppression list
- **list_bounces**: Useful for list cleaning.

Lists all bounced email records
- **get_template_details**: Retrieves details for a specific template
- **list_marketing_contacts**: Lists all marketing contacts
- **list_marketing_lists**: Lists all marketing contact lists
- **list_verified_senders**: Only verified senders can be used in the from_email field.

List all verified sender identities
- **list_dynamic_templates**: List all Dynamic Transactional Templates
- **dispatch_email**: Ensure you use a verified sender email in "from_email".

Sends an email via SendGrid SMTP relay
- **delete_spam_report**: Use with caution — sending to users who report spam can damage your sender reputation.

Remove an email from the spam report suppression list
- **search_contact_by_email**: Returns full contact profile including custom fields, lists, and segments.

Look up a marketing contact by email address
- **get_delivery_stats**: Use YYYY-MM-DD format.

Get global email delivery statistics
- **list_blocked_emails**: Different from bounces — blocks are typically temporary server-level rejections.

List all blocked email addresses
- **create_marketing_contact**: Merges data if the contact already exists.

Creates or updates a marketing contact
- **list_global_unsubscribes**: Lists global unsubscribes
- **list_spam_reports**: Lists user-reported spam complaints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twilio SendGrid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Using the SendGrid API, list emails that have bounced recently to audit our hygiene."

**🤖 AI Agent:**
> I've invoked `list_bounces` spanning your latest transmissions. You have exactly 4 hard-bounced targets stored within suppression parameters. For instance, 'hello@fake-email-z.com' returned an error string: 550 Relay Denied. Do you want me to automatically execute the `delete_bounce` directive on any specific valid records to unblock them?

---

**👤 You:**
> "Dispatch an HTML email from 'marketing@mybrand.com' to 'client@test.com' with subject 'Special Delivery'. Use standard <h1>."

**🤖 AI Agent:**
> The transmission has been completed effectively. The `dispatch_email` tool received identical constraints, leveraging 'marketing@mybrand.com'. The SendGrid HTTP payload accepted your outbound message synchronously and queued it upon the global outgoing rail successfully.

---

**👤 You:**
> "Audit the Dynamic Transactional Templates list. Summarize findings."

**🤖 AI Agent:**
> I've engaged `list_dynamic_templates` surveying your internal dashboard environment. Your vault holds 7 different distinct design layouts. The most recently updated is the 'Welcome Onboarding Form' attached to template ID (d-f018x8axxx...). Would you like me to dive into `get_template_details` for that specific iteration to reverse-engineer its internal blocks?


## ❓ FAQ

**Q: Can the agent automatically send emails on my behalf?**
Yes. The integration natively wraps the `dispatch_email` mutation tool. If adequately prompted, the system will formulate HTML payloads and broadcast them assuming you explicitly provide the verified Sender Identity (from_email) corresponding to your account.

**Q: How do I remove an email block suppressing one of my clients?**
You don't need to manually interact with the web app anymore. Dictate to the LLM: 'Unblock client@gmail.com from my bounce list'. The agent will instantly leverage `delete_bounce` removing the suspension logic behind the scenes.

**Q: Can I query spam complaints regarding my outgoing templates?**
Absolutely. Utilize the command prompt sequence to call `list_spam_reports`. It retrieves detailed events pointing precisely to domains triggering those complaints, empowering you to adjust or purge bad contacts dynamically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twilio-sendgrid](https://vinkius.com/mcp/twilio-sendgrid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twilio SendGrid** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twilio-sendgrid` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twilio SendGrid** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twilio-sendgrid": {
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
