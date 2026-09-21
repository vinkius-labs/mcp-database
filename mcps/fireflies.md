# Fireflies MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fireflies)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Turn your recorded meetings into work: transcripts, action items, speaking metrics and AskFred Q&A.

## Description
Connect any AI agent to **Fireflies** — the AI notetaker that joins your meetings, transcribes them and extracts what matters. No key of your own to borrow; bring your own Fireflies API key and read your own account.

### What you can do

- **Find a meeting** — list your transcripts, filtered by keyword, date window, host or participant, paged with skip/limit
- **Read the full meeting** — attendees, who joined and left when, and the AI summary: gist, overview, meeting type, action items, topics discussed, outline and keywords
- **Pull the action items** — the fastest route to the to-do list a meeting produced, with the outline for context
- **Read what was said** — the sentence stream with speaker, timestamp and AI tags (task, question, price, metric, date, sentiment), filterable by speaker, text or time window
- **See who talked** — per-speaker talk time, words per minute, longest monologue and filler-word count, plus overall sentiment
- **Ask Fred** — start a question thread about one meeting or across a range, read the answers and the suggested follow-ups

### Why it matters

The meeting ended an hour ago and nobody remembers what was decided. This reads the record: the decision, the owner and the moment it was said, with a timestamp the agent can quote.


## Available Tools (9)
- **ask_fred**: Ask either about one meeting (transcript_id) or across a range of meetings — pass exactly one of the two, never both, or Fireflies rejects it. Optional response_language is an ISO 639-1 code: en, pt, es, fr, de, ja and so on. The answer may arrive with status "processing" — poll it with get_askfred_thread.

Ask Fred a question about your meetings
- **get_meeting_action_items**: Same fields as get_meeting, trimmed to what a follow-up needs.

Pull the action items out of one meeting
- **get_askfred_thread**: Find the id with list_askfred_threads.

Read a full AskFred thread with its question and answer history
- **get_meeting_dialogue**: Narrow it with a speaker name, a search string or a time window in seconds from the start, then page through with offset/amount (defaults 0/60). Use this to quote a decision, find a number someone mentioned, or reconstruct who said what.

Read what was actually said in a meeting, line by line
- **get_meeting_metrics**: Useful for coaching, reviewing a demo, or seeing whether one person dominated the room.

Get speaking metrics and sentiment for a meeting
- **get_meeting**: Find the id with list_meetings first. For the line-by-line conversation use get_meeting_dialogue; for speaking metrics use get_meeting_metrics.

Get one meeting in full: attendees, attendance, summary, action items and topics
- **list_askfred_threads**: Filter by transcript_id to see the questions asked about one meeting, then read the answers with get_askfred_thread.

List AskFred question threads, optionally for one meeting
- **list_meetings**: Paginate with skip/limit (defaults 0/20). Filter by keyword (searches titles and, with scope, the spoken text), an ISO 8601 date window (from_date/to_date), a host or participant email, or mine=true for only the API key owner's meetings. Use get_meeting to read one meeting in full.

List your Fireflies meetings, newest first
- **list_team_members**: Page with offset/amount (defaults 0/50).

List the users in your Fireflies team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fireflies** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was decided in the product meeting yesterday?"

**🤖 AI Agent:**
> I listed the meetings from yesterday and opened the one titled for the product discussion. The summary's gist states the decision, the action items name the owners, and the topics-discussed list shows the alternatives that were rejected — so you get the outcome and what else was on the table.

---

**👤 You:**
> "Give me the action items from this morning's standup so I can put them in our tracker."

**🤖 AI Agent:**
> Pulled. The action-items tool returned the to-do list the meeting produced, with the outline underneath so each item keeps its context, and the keywords naming the systems and people involved. They are in the order they came up, ready to file one by one.

---

**👤 You:**
> "Find the exact moment the customer mentioned their budget and tell me what they said."

**🤖 AI Agent:**
> Found it. I opened the dialogue for that call, filtered the sentences on the budget term and got the line back with the speaker, a timestamp in minutes and seconds, and the price tag Fireflies attached to it — so you can quote the number and the moment it was said.


## ❓ FAQ

**Q: Do I need an API key?**
Yes. Fireflies' GraphQL API authenticates every call. Generate a key at fireflies.ai → Settings → Integrations → API Keys, paste it into the credential field, and it is sent as "Authorization: Bearer <key>".

**Q: Can I read the actual spoken words, not just the summary?**
Yes. get_meeting_dialogue returns the sentence stream with speaker, start and end time, and AI tags marking tasks, questions, prices, metrics, dates and sentiment. Filter it by speaker, a search string or a time window in seconds, then page through with offset/amount.

**Q: How do I find the meeting id Fireflies uses?**
Run list_meetings with a date window, a host or participant email, or a keyword. It returns the transcript id alongside the title, date, duration and action-item count. Pass that id to get_meeting or any other tool.

**Q: What is the difference between get_meeting and ask_fred?**
get_meeting returns the record Fireflies already built — the summary, action items, outline and attendees. ask_fred starts a new question thread in natural language, about one meeting (transcript_id) or across a range, and returns an answer plus suggested follow-ups you can continue with get_askfred_thread.

**Q: Can I see how much each person talked?**
Yes. get_meeting_metrics returns per-speaker talk time and its percentage of the meeting, word count, words per minute, monologue count and longest monologue, filler-word count, plus the overall sentiment split and how many questions, dates, metrics and tasks were detected.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fireflies](https://vinkius.com/en/ai-agent-connect/fireflies)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fireflies** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fireflies` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fireflies** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fireflies": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
