# Amplemarket MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplemarket)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Sales automation and lead generation — manage sequences, leads, and custom signals via AI.

## Description
Connect your **Amplemarket** account to your AI agent to unlock professional sales automation and lead orchestration. Amplemarket is an all-in-one sales platform that helps B2B teams find and engage their next customers. By integrating Amplemarket with your AI agent, you can automate complex outbound strategies through simple natural language commands. From searching for high-intent B2B contacts to managing outreach sequences and triggering custom Duo Copilot signals, your agent handles your outbound sales strategy seamlessly.

Using this Amplemarket MCP server, your AI agent gains the ability to discover new leads based on specific firmographic or intent criteria. You can search for people by job title, company name, or other professional attributes. Once discovered, your agent can manage these leads by creating lead lists and adding contacts to them, keeping your prospecting efforts organized. This powerful integration between Amplemarket and your AI agent ensures that your sales pipeline is always full of high-quality prospects.

Furthermore, the Amplemarket integration allows your AI agent to orchestrate outreach sequences. You can list available sequences and programmatically add new leads to them, ensuring consistent follow-ups without manual intervention. For advanced sales playbooks, your agent can trigger custom signals in Duo Copilot by pushing dynamic data entries via webhook tokens. This enables highly personalized and automated engagement strategies that adapt to your leads' behavior in real-time.

### What you can do

- **Lead Discovery** — Search for people and retrieve detailed contact profiles using specific firmographic or intent criteria directly through your AI agent.
- **List Management** — Create and manage lead lists to organize your prospecting efforts within Amplemarket effortlessly.
- **Sequence Orchestration** — List available outreach sequences and add new leads to them programmatically using natural language.
- **Custom Signals (Duo Copilot)** — Trigger custom automated playbooks by pushing dynamic data entries via webhook tokens to Amplemarket's Duo Copilot.
- **Sales Insights** — Quickly look up contact details or identify active sequences directly from your chat interface with the help of your AI agent.

### How it works

1. **Subscribe** — Add the Amplemarket MCP server to your AI agent's workspace.
2. **Authenticate** — Enter your Amplemarket API Key to securely connect your account.
3. **Engage** — Start managing your sales outreach and prospecting through Claude, Cursor, or any MCP-compatible client using natural conversation.

### Who is this for?

- **Sales Development Reps (SDRs)** — Automate lead addition to sequences and research prospects effortlessly using an AI agent.
- **Sales Managers** — Monitor active sequences and manage lead lists on the fly within Amplemarket.
- **Growth Hackers** — Trigger Custom Signals based on external intent data to launch personalized playbooks via your AI agent.
- **RevOps Specialists** — Verify API integrations and inspect JSON lead profiles using simple commands in your chat interface.


## Available Tools
- **search_people**: Search for B2B contacts
- **find_person**: Find specific person
- **list_lead_lists**: List lead lists
- **create_lead_list**: Create a lead list
- **add_leads_to_list**: Add leads to a list
- **list_sequences**: List active sequences
- **add_leads_to_sequence**: Add leads to sequence
- **trigger_custom_signal**: Trigger custom signal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplemarket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for people with job title 'VP of Sales'."

**🤖 AI Agent:**
> I've searched for 'VP of Sales' in Amplemarket. I found 15 matching profiles. The top results include executives from tech companies. Would you like me to add these profiles to a specific lead list?

---

**👤 You:**
> "List my active outreach sequences."

**🤖 AI Agent:**
> I've retrieved your Amplemarket sequences. You currently have 3 active sequences: 'Q1 Enterprise Outreach', 'Inbound Demo Follow-up', and 'Webinar Attendees'. Which sequence would you like to inspect?

---

**👤 You:**
> "Trigger custom signal 'sig_123' with email 'lead@example.com' and variable 'Product A'."

**🤖 AI Agent:**
> I've successfully pushed the data entry to Amplemarket's custom signal sig_123. Duo Copilot will now evaluate the signal and automatically generate the personalized sequence for lead@example.com based on your playbook rules.


## ❓ FAQ

**Q: Can I target specific industries with my lead search?**
Yes! You can use your AI agent to search for people by job title, company name, and other intent-based signals within the Amplemarket database.

**Q: How does the Duo Copilot signal work?**
Duo Copilot uses Custom Signals to trigger automated playbooks. Your agent sends dynamic data to a specific signal token, and Amplemarket handles the personalized engagement logic.

**Q: Does adding a lead to a sequence update existing data?**
No, the sequence orchestration tool only adds new leads to the specified sequence. It does not modify existing lead information already present in Amplemarket.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplemarket](https://vinkius.com/mcp/amplemarket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Amplemarket** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `amplemarket` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Amplemarket** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "amplemarket": {
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
