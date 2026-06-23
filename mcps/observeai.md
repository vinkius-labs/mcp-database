# Observe.AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/observeai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze and evaluate contact center interactions via Observe.AI — track transcripts, QA scores, and coaching directly from your AI agent.

## Description
Connect your **Observe.AI** account to your AI agent and gain deep visibility into your contact center performance and conversation intelligence through natural conversation.

### What you can do

- **Interaction Monitoring** — List and inspect all calls, chats, and emails processed by the platform, including metadata and analysis.
- **Full Transcripts** — Retrieve the complete text transcripts for any call or chat interaction for detailed review.
- **QA & Evaluations** — Access quality assurance scores, evaluation forms, and individual agent performance metrics.
- **AI Insights** — View automated interaction summaries and identified business moments (e.g., Greetings, Objections).
- **Coaching Oversight** — Monitor agent coaching sessions and feedback logs to track improvement.
- **Workspace Management** — List all agents, supervisors, and admins in your Observe.AI instance.

### How it works

1. Subscribe to this server
2. Enter your Observe.AI API Key (Bearer Token)
3. Start analyzing your contact center intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **QA Analysts** — quickly check evaluation scores or read transcripts without opening the portal.
- **Contact Center Managers** — monitor high-level performance trends and AI-generated summaries during daily standups.
- **Coaches & Supervisors** — verify coaching session history and agent progress through natural language.


## Available Tools (10)
- **get_evaluation_details**: Get specific evaluation info
- **get_interaction_details**: Get specific interaction info
- **get_interaction_transcript**: Get interaction transcript
- **list_coaching_sessions**: List agent coaching sessions
- **list_qa_evaluations**: List QA evaluations
- **list_evaluation_forms**: List QA evaluation forms
- **list_interactions**: AI.

List contact center interactions
- **list_interaction_moments**: g. Greeting, Closing) across interactions.

List identified key moments
- **list_interaction_summaries**: List AI-generated summaries
- **list_workspace_users**: AI workspace.

List workspace agents and users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Observe.AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent call interactions from today."

**🤖 AI Agent:**
> Retrieving interactions... I found 12 calls from today. Notable ones include 'Interaction #98765' (Duration: 5:30, Sentiment: Positive) and 'Interaction #98766' (Sentiment: Frustrated). Would you like the transcript for the frustrated call?

---

**👤 You:**
> "What is the QA score for interaction ID 'int_12345'?"

**🤖 AI Agent:**
> Fetching evaluation details... The interaction int_12345 received a total QA score of 95%. It scored perfectly on 'Compliance' and 'Empathy', with a minor deduction in 'Resolution Speed'. Shall I list the full evaluator feedback?

---

**👤 You:**
> "Show me the AI summaries for our latest interactions."

**🤖 AI Agent:**
> Retrieving AI summaries... I found 5 recent summaries. The overall theme focuses on 'Renewals' and 'Billing Inquiries'. One summary identifies a recurring issue with 'Portal Login'. Would you like the detailed summary for that specific case?


## ❓ FAQ

**Q: How do I get an Observe.AI API Key?**
You can find your API Key in the Observe.AI dashboard under Settings > API Keys. This token is used as a Bearer Token for authentication.

**Q: Can I read full call transcripts through the agent?**
Yes! Use the `get_interaction_transcript` tool with a specific Interaction ID to retrieve the full text content of the conversation.

**Q: What information is included in the QA evaluations?**
Evaluations include the QA form used, individual section scores, overall score, and specific feedback or comments provided by the evaluator.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/observeai](https://vinkius.com/mcp/observeai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Observe.AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `observeai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Observe.AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "observeai": {
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
