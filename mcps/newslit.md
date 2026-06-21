# Newslit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/newslit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track news coverage, analyze media impact, and discover press opportunities with media intelligence tools for communications teams.

## Description
Connect your **Newslit** account to any AI agent and take full control of your news monitoring and market intelligence through natural conversation. Newslit provides a powerful News API for generating targeted news briefs and story collections, and this integration allows you to retrieve report metadata, create customized monitoring filters, and ingest real-time news stories directly from your chat interface.

### What you can do

- **Report & Monitoring Orchestration** — List all managed news reports and retrieve detailed configuration metadata programmatically to ensure your research setup is always synchronized.
- **Targeted Story Intelligence** — Fetch the latest news stories and headlines associated with your reports directly from the AI interface to track industry trends and competitors.
- **Custom Report Control** — Create, update, and delete customized news reports with specific topic filters and exclusions via natural language to drive better research efficiency.
- **Media Discovery Oversight** — Retrieve stories with detailed source information and direct links to the original articles using simple AI commands.
- **Operational Monitoring** — Track system responses and manage report metadata to ensure your news intelligence is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Newslit API Key from your dashboard integration settings
3. Start monitoring news from Claude, Cursor, or any MCP-compatible client

No more manual browsing through news sites for industry updates. Your AI acts as a dedicated news analyst or market researcher.

### Who is this for?

- **Market Researchers** — quickly retrieve industry summaries and monitor competitor activity without switching apps.
- **PR & Communications Teams** — automate the collection of news mentions and track brand reputation via natural conversation.
- **Product Managers** — streamline the retrieval of sector trends and monitor technological shifts directly within the chat.


## Available Tools
- **create_report**: Pass report data as a JSON string.

Create a new news report
- **delete_report**: Delete a news report
- **get_report**: Get report details
- **list_reports**: List all news reports
- **list_stories**: Retrieve news stories from a report
- **update_report**: Update an existing report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Newslit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my news reports in Newslit."

**🤖 AI Agent:**
> I've retrieved your reports. You have 3 active environments: 'Tech Trends', 'Industry Rivals', and 'Sustainability'. Which one would you like to see stories from?

---

**👤 You:**
> "Get the full details and story coverage for report ID rpt_4521."

**🤖 AI Agent:**
> Report "Q1 Brand Mentions" (rpt_4521) contains 147 stories collected over the last 90 days. Top sources include Reuters (12 mentions), TechCrunch (8 mentions), and Bloomberg (6 mentions). Overall sentiment is 72% positive, 18% neutral, and 10% negative.

---

**👤 You:**
> "Create a new media monitoring report tracking mentions of artificial intelligence in tech news."

**🤖 AI Agent:**
> Your new report "AI Media Monitor" has been created successfully with ID rpt_4589. It is configured to track the keyword "artificial intelligence" across all indexed tech news sources. Initial results are being collected and should populate within the next few minutes.


## ❓ FAQ

**Q: Can my AI automatically find the latest stories for a specific report by its ID?**
Yes! Use the `list_stories` tool with the Report ID. Your agent will respond with complete metadata for the newest stories, including headlines, summaries, and source links in seconds.

**Q: How do I find my Newslit API Key?**
Log in to your Newslit account, navigate to **Integrations** > **News API**, and you will find your unique secret token (X-NewslitApiKey) there.

**Q: Does the API provide full article text?**
The API primarily provides headlines, curated summaries, and source metadata. Direct links are provided to access the full content on the original publisher's website.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/newslit](https://vinkius.com/mcp/newslit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Newslit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `newslit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Newslit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "newslit": {
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
