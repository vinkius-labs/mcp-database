# Goodcall MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goodcall)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Answer business phone calls with an AI receptionist that schedules appointments, takes messages, and never puts callers on hold.

## Description
Connect your **Goodcall** account to any AI agent and manage your virtual phone agent fleet through natural conversation.

### What you can do

- **Agent Management** — List all virtual phone agents, inspect individual configurations, and update greeting scripts or behavior settings
- **Call History** — Browse all calls handled by AI agents, filter by specific agent, and inspect individual call details
- **Transcripts & Summaries** — Retrieve full conversation transcripts and AI-generated call summaries with key topics and outcomes
- **Missed Call Tracking** — Identify calls that were missed or abandoned for follow-up prioritization
- **Booking Management** — View all appointments booked by the AI agent during customer calls
- **FAQ Configuration** — List all FAQ entries configured for each agent to verify knowledge coverage
- **Performance Analytics** — Track aggregate metrics including total calls, answer rate, booking conversion, and trends

### How it works

1. Subscribe to this server
2. Enter your Goodcall API Key from your account settings
3. Start managing your phone agents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — monitor how the AI receptionist handles calls, check bookings, and follow up on missed calls
- **Operations Managers** — analyze call volume, answer rates, and booking conversions across all phone agents
- **Customer Service Leaders** — review call transcripts, refine agent scripts, and ensure FAQ coverage


## Available Tools (13)
- **check_goodcall_status**: Verify connectivity
- **get_agent**: Get agent details
- **get_analytics**: Get call analytics
- **get_call_summary**: Get call summary
- **get_call**: Get call details
- **get_transcript**: Get call transcript
- **list_agents**: List AI agents
- **list_bookings**: List bookings
- **list_calls_by_agent**: List calls by agent
- **list_calls**: List all calls
- **list_faqs**: List FAQs
- **list_missed_calls**: List missed calls
- **update_agent**: Update an agent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Goodcall** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all calls from today and highlight any missed calls that need follow-up."

**🤖 AI Agent:**
> Today's call summary: 18 total calls handled by your AI agents. 15 answered successfully (83.3% answer rate), 3 missed calls. Missed calls needing follow-up: 1) +1 (555) 234-5678 at 9:14 AM — rang 4 times, no pickup. 2) +1 (555) 876-5432 at 11:02 AM — caller hung up during greeting. 3) +1 (555) 345-6789 at 2:30 PM — voicemail left. 2 bookings made today. Would you like to see the call transcripts or update the agent scripts?

---

**👤 You:**
> "Show me the summary and transcript of the last call handled by the main office agent."

**🤖 AI Agent:**
> Last call for 'Main Office Agent' (agent_001): call_5678, duration 3m 42s, caller: +1 (555) 901-2345. AI Summary: Customer called about business hours and pricing for a dental cleaning. The agent confirmed operating hours (Mon-Fri 8AM-6PM, Sat 9AM-2PM) and quoted $120 for a standard cleaning. Customer booked an appointment for Thursday at 10AM. Outcome: booking completed. Transcript available — 14 exchanges between caller and agent. Would you like to read the full transcript or check the FAQ entries?

---

**👤 You:**
> "Show analytics for all my agents this month — answer rates, bookings, and total call volume."

**🤖 AI Agent:**
> Monthly analytics: Total calls: 342. Answer rate: 89.5% (306 answered, 36 missed). Bookings: 78 appointments made (25.5% booking conversion). Average call duration: 2m 48s. Peak hours: 10-11 AM (52 calls) and 2-3 PM (41 calls). Agent breakdown: 1) 'Main Office' — 198 calls, 92% answer rate, 45 bookings. 2) 'After Hours' — 89 calls, 85% answer rate, 22 bookings. 3) 'Spanish Line' — 55 calls, 87% answer rate, 11 bookings. Would you like to update agent scripts or review missed calls?


## ❓ FAQ

**Q: Can I review what my AI phone agent said during a customer call?**
Yes. Use `get_transcript` with a Call ID to retrieve the full conversation transcript between the AI agent and the caller. For a quick overview, use `get_call_summary` which provides an AI-generated summary with key topics discussed and the call outcome (e.g., booking made, question answered, callback requested).

**Q: Can I track missed calls and see which ones need follow-up?**
Yes. The `list_missed_calls` tool retrieves all calls that were missed or abandoned, including caller phone number, timestamp, and any partial interaction data. This helps you prioritize follow-up callbacks and identify peak call times when your agents may be overloaded.

**Q: Can I see appointments booked by the AI agent during calls?**
Yes. The `list_bookings` tool retrieves all appointments booked by the AI agent during customer calls, including date, time, caller details, and the associated call ID. Use `get_analytics` to track your booking conversion rate — the percentage of calls that result in a scheduled appointment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goodcall](https://vinkius.com/mcp/goodcall)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Goodcall** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `goodcall` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Goodcall** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "goodcall": {
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
