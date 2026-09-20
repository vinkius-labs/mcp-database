# Google Slides MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/google-slides)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Read, create, and edit Google Slides decks — a full presentation workflow for any AI agent through the official Slides API.

## Description
Connect your **Google Slides** decks to any AI agent through the official Google Slides API. Your agent can open a presentation, read it as structure or plain text, build new decks, add slides, and apply text edits across the whole file.

### What you can do

- **Read** — Fetch a presentation's structure (title, slides, object IDs) or its flat plain text
- **Create** — Start a new deck with a title
- **Build** — Add slides with a chosen layout (title, section-header, title-and-body, blank)
- **Edit** — Fill a slide with text or run find-and-replace across the entire deck

### How it works

1. Create a Google Cloud project, enable the Slides API, and create OAuth 2.0 client credentials (Web application)
2. Paste the Client ID and Client Secret into this server's credential fields
3. Connect your Google account through OAuth — the agent then acts only on decks that account can access

### Who is this for?

- **Teams & Presenters** — let an agent turn notes or data into a deck, standardize wording across slides, and keep titles consistent
- **Automation** — generate branded starting decks from templates of layout choices, and update recurring slides without opening Slides


## Available Tools (6)
- **add_slide**: Layouts: title, section-header, title-and-body, blank (default). Use to build a deck slide by slide, then fill each slide with set_slide_text using the returned object ID.

Add a new slide to a Google Slides presentation
- **create_presentation**: Use when the user asks to start a fresh presentation or to turn agent-generated content into a deck. The title seeds the first slide.

Create a new Google Slides presentation
- **get_presentation**: Use when the agent needs to understand a deck before editing it, or when the user asks what is in a presentation. The presentation ID is the long code in the /edit/ URL — not the URL itself. For plain text instead of structure, use get_presentation_text.

Read the structure of a Google Slides presentation
- **get_presentation_text**: Use when the user wants to read, quote, or summarize a deck, or when the agent needs the text to find content. Layout and shapes are dropped — use get_presentation when structure matters.

Read the plain text of a Google Slides presentation
- **replace_slide_text**: Use for find-and-rename across slides: updating a brand name, a date, or a title. Empty replacement deletes all matches. The match is a plain-text or regex pattern over the whole presentation.

Replace matching text across a presentation
- **set_slide_text**: Use to fill a slide with content. Note it inserts at the end of the slide's text — to change existing text use replace_slide_text.

Set the text on a specific slide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Slides** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Turn these meeting notes into a 5-slide deck."

**🤖 AI Agent:**
> Created 'Board sync — Sep 2026' with 5 slides: a title slide, then section headers 'Decisions', 'Open items', 'Risks', and a closing 'Next steps'. Filled each slide with the notes, grouped by theme. Want me to rename any slide or tighten the wording?

---

**👤 You:**
> "Read my 'Investor update' deck and summarize what each slide says."

**🤖 AI Agent:**
> The deck has 7 slides: 1) cover with the quarter, 2) KPIs — MRR up 18% QoQ, churn steady, 3) product roadmap with two GA dates, 4) the enterprise pipeline by stage, 5) two hires highlighted, 6) risks — two flagged in red, 7) ask — board approval for the pricing change. Slides 2 and 6 are the ones investors will poke at.

---

**👤 You:**
> "Replace every 'ACME Inc' in the deck with 'Acme Corp' and make it official."

**🤖 AI Agent:**
> Replaced 6 occurrences of 'ACME Inc' with 'Acme Corp' across all slides in one pass. The deck now reads consistently with the new name. Nothing else changed.


## ❓ FAQ

**Q: Which Google Cloud permissions are required?**
The OAuth flow requests only the Google Slides API scope. The agent can therefore read and modify presentations that your connected Google account can access, and nothing beyond that scope.

**Q: How do I get the presentation ID and slide object IDs?**
The presentation ID is the long code in the /edit/ URL. Slide object IDs are not visible in the browser — call get_presentation to list them, or add_slide returns the new slide's ID. set_slide_text needs that object ID, not the browser slide number.

**Q: Can it rebuild an entire deck from scratch?**
Yes: create the presentation, then loop add_slide (choosing a layout each time) and set_slide_text on each returned object ID. This builds a working deck slide by slide. Complex layouts, charts and images are out of scope — this is a text-first workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/google-slides](https://vinkius.com/en/ai-agent-connect/google-slides)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Slides** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-slides` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Slides** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-slides": {
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
