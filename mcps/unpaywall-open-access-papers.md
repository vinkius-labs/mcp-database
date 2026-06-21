# Unpaywall (Open Access Papers) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unpaywall-open-access-papers)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access millions of open-access scholarly articles. Check OA status and retrieve full-text PDF links using DOIs.

## Description
Connect to the **Unpaywall** database to instantly find legal, open-access versions of scholarly papers. This server allows your AI agent to bypass paywalls by locating freely available PDFs and repository versions of research articles using their Digital Object Identifier (DOI).

### What you can do

- **OA Status Verification** — Instantly check if a specific scholarly article is available for free under an Open Access license.
- **PDF Retrieval** — Get direct links to legal, full-text PDF versions of research papers hosted on publisher sites or institutional repositories.
- **Metadata Inspection** — Retrieve information about the type of Open Access (gold, green, bronze, etc.) and the hosting source.
- **Research Automation** — Streamline literature reviews by letting your agent automatically find accessible versions of cited works.

### How it works

1. Subscribe to this server
2. Enter your email address (required by Unpaywall's API policy)
3. Start searching for open-access papers in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Academics** — quickly find full-text versions of papers without navigating multiple library portals
- **Students** — access required reading materials that are legally available for free
- **Data Scientists** — automate the collection of open-access research data and papers for analysis


## Available Tools
- **get_article_oa_status**: Retrieve Open Access status and locations for a specific DOI


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unpaywall (Open Access Papers)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the Open Access status for DOI 10.1038/nature12345."

**🤖 AI Agent:**
> I've checked the Unpaywall database for DOI 10.1038/nature12345. This article is available via Open Access. You can download the full PDF here: [Link].

---

**👤 You:**
> "Find a free version of the paper with DOI 10.1126/science.1234567."

**🤖 AI Agent:**
> Searching... I found a legal, open-access version of this paper hosted on a university repository. Here is the link to the full text.

---

**👤 You:**
> "Is the article 10.1016/j.cell.2021.01.001 behind a paywall?"

**🤖 AI Agent:**
> According to Unpaywall, this specific DOI is currently not available as a free Open Access version. It appears to be behind a publisher paywall.


## ❓ FAQ

**Q: How do I check if a specific research paper is available for free?**
Use the `get_article_oa_status` tool with the paper's DOI. Your agent will query the Unpaywall database and return the Open Access status along with direct links to the PDF if available.

**Q: Does this tool provide legal versions of the papers?**
Yes. Unpaywall only indexes legal, author-archived, or publisher-provided Open Access versions of scholarly articles. It does not access pirated content.

**Q: What information is required to use this server?**
You need the DOI (Digital Object Identifier) of the article and a valid email address to authenticate with the Unpaywall API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unpaywall-open-access-papers](https://vinkius.com/mcp/unpaywall-open-access-papers)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Unpaywall (Open Access Papers)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `unpaywall-open-access-papers` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Unpaywall (Open Access Papers)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unpaywall-open-access-papers": {
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
