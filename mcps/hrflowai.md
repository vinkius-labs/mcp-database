# HrFlow.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hrflowai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

AI-powered talent acquisition API for parsing, matching, and reasoning.

## Description
Empower your AI agents with HrFlow.ai's advanced talent acquisition capabilities. This MCP server allows you to parse resumes, search profiles and jobs with semantic filters, score candidates against job descriptions, and ask natural language questions about profiles. Ideal for automating recruitment workflows with AI-driven insights.


## Available Tools
- **ask_profile**: Asks a natural language question about a specific profile
- **list_boards**: Lists job boards
- **list_jobs**: Lists jobs stored in HrFlow boards
- **list_profiles**: Lists candidate profiles stored in HrFlow
- **list_sources**: Lists profile sources
- **parse_profile**: Parses a resume file into a structured profile
- **score_profiles**: Scores candidate profiles against a specific job
- **search_jobs**: Searches for jobs with semantic filters
- **search_profiles**: Searches for profiles with semantic filters
- **unfold_profile**: Analyzes and unfolds the career path of a profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HrFlow.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 profiles added to my HrFlow source."

**🤖 AI Agent:**
> I'll fetch the latest profiles for you.

---

**👤 You:**
> "Ask profile key 'abc-123' if they have experience with Kubernetes."

**🤖 AI Agent:**
> I'll analyze the candidate's profile and answer your question.

---

**👤 You:**
> "Find jobs that match candidate 'john-doe-key'."

**🤖 AI Agent:**
> I'll use semantic search to find matching jobs for this candidate.


## ❓ FAQ

**Q: How do I get HrFlow API credentials?**
You can find your X-API-KEY in the HrFlow dashboard under Settings > API. You also need the email address of your account.

**Q: Can I parse PDF resumes with this MCP?**
Yes, the parse_profile tool allows you to provide a public URL to a resume file for AI parsing.

**Q: What is profile asking?**
It's an AI feature that lets you ask questions about a candidate's profile in plain English and get intelligent answers based on their data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hrflowai](https://vinkius.com/mcp/hrflowai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HrFlow.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hrflowai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HrFlow.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hrflowai": {
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
