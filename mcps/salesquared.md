# Salesquared MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesquared)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate business communications via Salesquared — manage SMS, voice calls, and leads directly with AI.

## Description
Connect your **Salesquared** account to any AI agent and take full control of your multi-channel business communication through natural conversation. Salesquared provides a unified platform for SMS marketing, voice orchestration, and lead management, and this integration allows you to send automated messages, trigger voice OTPs, and manage your sales database directly from your chat interface.

### What you can do

- **SMS & Messaging Orchestration** — Send individual or bulk SMS messages programmatically to ensure your outreach is always synchronized.
- **Voice & OTP Intelligence** — Trigger automated voice calls and send secure voice OTPs directly from the AI interface to verify user identities.
- **Lead & Campaign Control** — List and manage your lead database and monitor active marketing campaigns via natural language.
- **Email Validation & Data Quality** — Verify email addresses programmatically to maintain high deliverability rates and ensure your contact data is accurate.
- **Operational Monitoring** — Access conference call controls and retrieve system metadata using simple AI commands to streamline your communications.

### How it works

1. Subscribe to this server
2. Enter your Salesquared API Key from your account settings
3. Start managing your communications and leads from Claude, Cursor, or any MCP-compatible client

No more manual texting or switching between telephony tools. Your AI acts as a dedicated communications manager or sales automation coordinator.

### Who is this for?

- **Sales & Marketing Teams** — quickly send promotional SMS and monitor campaign responses without switching apps.
- **Support & Operations** — automate the delivery of voice OTPs and validate customer emails via natural conversation.
- **Developers** — integrate multi-channel communication capabilities into custom AI-driven business workflows.


## Available Tools (11)
- **conference_mute**: Mute or unmute a participant
- **create_audio_from_tts**: Create audio from text
- **create_lead**: Create a new lead
- **create_voice_survey**: Create a voice survey
- **get_campaign**: Get details for a specific campaign
- **get_lead**: Get lead details
- **list_campaigns**: List campaigns
- **list_leads**: List all leads
- **send_sms**: Send an SMS message
- **send_voice_otp**: Send a Voice OTP
- **validate_email**: Validate an email address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesquared** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS broadcast to my new leads: 'Welcome to our platform!'."

**🤖 AI Agent:**
> SMS broadcast initiated! I've sent the message to your recent leads via Salesquared. Should I track the delivery status for you?

---

**👤 You:**
> "Show me all active SMS and voice campaigns with their delivery and conversion metrics."

**🤖 AI Agent:**
> 6 active campaigns. SMS (4): "Flash Sale Alert" sent 3,400 messages (97% delivered, 12% clicked, $8,900 revenue). "Appointment Reminder" sent 890 (98% delivered, reduced no-shows by 45%). "Payment Reminder" sent 234 (96% delivered, 34% paid within 24h). "Welcome Series" sent 567 (97% delivered, 28% engaged). Voice (2): "Lead Qualification" made 145 calls (78% answered, 34% qualified). "Survey" completed 89 of 120 calls (74% completion). Total revenue attributed: $14,200.

---

**👤 You:**
> "Send a bulk SMS campaign to all leads tagged as hot prospects with a meeting booking link."

**🤖 AI Agent:**
> SMS campaign sent to 156 hot prospect leads. Message: "Hi [Name], we'd love to show you how our platform can help your team. Book a personalized demo at your convenience: [booking_link]. Reply STOP to opt out." Delivery: 153 delivered (98.1%), 3 undeliverable. Personalization: first name and company name injected. Booking link: unique per recipient for tracking. Based on similar campaigns, expect 18-22 bookings (12-14% conversion). Campaign cost: $23.40.


## ❓ FAQ

**Q: Can my AI automatically send a Voice OTP to verify a user's mobile number?**
Yes! Use the `send_voice_otp` tool. Provide the mobile number and the OTP code, and your agent will trigger an automated call to deliver the security code instantly.

**Q: How do I find my Salesquared API Key?**
Log in to your Salesquared dashboard, navigate to the API or Developer section, and you will find your unique secret API Key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesquared](https://vinkius.com/mcp/salesquared)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesquared** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salesquared` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesquared** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesquared": {
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
