# Thesaurus API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thesaurus-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search synonyms and antonyms — audit linguistics via AI.

## Description
Empower your AI agent to orchestrate your entire linguistic research and writing auditing workflow with the **Thesaurus API**, the specialized source for programmable synonym and antonym data. By connecting the APIVerve-powered thesaurus service to your agent, you transform complex word searches into a natural conversation. Your agent can instantly retrieve synonyms and antonyms for any word and query specific linguistic distributions without you ever touching a dictionary portal. Whether you are conducting academic research or managing content creation constraints, your agent acts as a real-time linguistic consultant, ensuring your data is always expressive and precise.

### What you can do

- **Word Auditing** — Retrieve high-resolution synonyms and antonyms for any specific word and maintain a clear view of vocabulary distribution.
- **Linguistic Oversight** — Audit multiple word meanings to understand the semantic reach of your content instantly.
- **Metadata Intelligence** — Retrieve unique linguistic markers for any record to assist in deep-dive archival classification.
- **Operational Monitoring** — Check API status to ensure your writing research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your APIVerve API Key
3. Start managing your linguistic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Editors** — monitor vocabulary trends and retrieve fresh synonyms straight from your workflow.
- **Linguists & Students** — verify word relations and audit semantic patterns without manual searching.
- **Content Creators** — perform rapid audits of linguistic markers and identify relevant stylistic patterns through natural language.
- **Operations Leads** — automate creative data querying to orchestrate cross-functional writing teams smoothly.


## Available Tools
- **check_api_status**: Check if the Thesaurus service is operational
- **get_synonyms_antonyms**: Get synonyms and antonyms for a specific word


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thesaurus API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find synonyms for the word 'beautiful' using Thesaurus API."

**🤖 AI Agent:**
> I've retrieved the synonyms for 'beautiful'! Notable entries include 'attractive', 'lovely', and 'stunning'. Would you like the antonyms or another word audit?

---

**👤 You:**
> "What is the antonym of 'success'?"

**🤖 AI Agent:**
> I've identified the antonyms for 'success'! The primary marker is 'failure'. I can provide the full list of synonyms if you'd like to maintain stylistic control over your content.

---

**👤 You:**
> "Check the status of the Thesaurus service."

**🤖 AI Agent:**
> I've checked the status of the APIVerve Thesaurus service! It is currently identified as 'active' and fully operational. I can assist you with vocabulary retrieval for your writing projects.


## ❓ FAQ

**Q: How do I find my APIVerve Key?**
Log in to your [**APIVerve dashboard**](https://apiverve.com/), and you will find your API Key in your account settings. Copy and paste it below.

**Q: Does it support multiple languages?**
This specific API focuses on English synonyms and antonyms metadata.

**Q: Can the agent show both synonyms and antonyms?**
Yes. The `get_synonyms_antonyms` tool retrieves both lists for the specified word where available in the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thesaurus-api](https://vinkius.com/mcp/thesaurus-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thesaurus API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `thesaurus-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thesaurus API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thesaurus-api": {
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
