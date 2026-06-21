# Guestmeter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guestmeter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Automate guest feedback collection and reputation management via Guestmeter directly from any AI agent.

## Description
Connect your **Guestmeter** hospitality feedback platform to any AI agent and take full control of your reputation management workflows through natural conversation.

### What you can do

- **Automated Surveys** — Trigger satisfaction surveys via Email or SMS for guests immediately after checkout.
- **Feedback Monitoring** — List and inspect all guest ratings, comments, and NPS types (Promoters, Passives, Detractors).
- **Reputation Insights** — Retrieve detailed reports on specific guest experiences to identify areas for improvement.
- **Real-time Alerts** — Stay updated on the most recent feedback entries to respond quickly to guest concerns.
- **Segmented Analysis** — Filter feedback to focus on your happiest guests (Promoters) or those needing attention (Detractors).

### How it works

1. Subscribe to this server
2. Enter your Guestmeter API Key and Secret Key
3. Start managing your guest feedback from Claude, Cursor, or any MCP-compatible client

No more manual review mining. Your AI assistant acts as a dedicated guest relations manager or reputation specialist.

### Who is this for?

- **Hotel Managers** — instantly retrieve daily feedback summaries and identify service gaps.
- **Front Office Teams** — automate survey triggers and check guest satisfaction scores during follow-ups.
- **Hospitality Group Executives** — monitor reputation trends across multiple properties from a single interface.


## Available Tools
- **get_guest_details**: Retrieve detailed information for a specific guest ID
- **list_detractors**: List all guests who are detractors (ratings 1-6)
- **list_guest_feedback**: List all guests and their feedback status/results
- **list_promoters**: List all guests who are promoters (ratings 9-10)
- **list_recent_feedback**: List the 50 most recent feedback entries
- **send_survey**: Requires either an email or phone number.

Trigger a new guest satisfaction survey via Email or SMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guestmeter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent guest feedback entries."

**🤖 AI Agent:**
> I've retrieved the latest entries. Recent feedback includes: Sarah J. [10/10] - 'Amazing stay!', Mark T. [8/10] - 'Good location, but room was small', and Elena R. [9/10] - 'Excellent service'. Would you like to see the full details for Sarah's review?

---

**👤 You:**
> "Send a survey to John Doe at john.doe@example.com for room 302."

**🤖 AI Agent:**
> Survey trigger sent! I've successfully requested a satisfaction survey for John Doe (Room 302) via email. Guestmeter will deliver it shortly.

---

**👤 You:**
> "Show me all our detractors from the last batch."

**🤖 AI Agent:**
> Analyzing feedback... I found 2 detractors in your recent records: Michael S. [5/10] - 'Check-in was slow' and Linda K. [4/10] - 'AC was noisy'. Would you like their contact IDs to follow up?


## ❓ FAQ

**Q: How do I find my Guestmeter API credentials?**
Log in to your Guestmeter dashboard and navigate to **Channels > Integration**. You will find your unique `apiKey` and `secretKey` there.

**Q: Can I trigger surveys for both email and SMS?**
Yes! The `send_survey` tool allows you to provide either a `guest_email` or a `guest_phone` number. Guestmeter will automatically deliver the survey via the provided channel.

**Q: How does the integration categorize guests into Promoters or Detractors?**
The integration uses the Net Promoter Score (NPS) logic: guests rating 9-10 are Promoters, 7-8 are Passives, and 1-6 are Detractors. You can use specialized tools like `list_promoters` to quickly access these segments.

**Q: Is the survey delivery instant?**
Yes, once the `send_survey` action is triggered, Guestmeter processes the request immediately and sends the invitation to the guest.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guestmeter](https://vinkius.com/mcp/guestmeter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Guestmeter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `guestmeter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Guestmeter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guestmeter": {
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
