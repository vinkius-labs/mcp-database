# Surfer SEO MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/surfer-seo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Connect your AI to Surfer SEO. Generate Content Editors, perform NLP SERP audits, and extract high-ranking keyword guidelines directly from the terminal.

## Description
Bring industry-leading organic search optimization strategies dynamically into your conversational workflows with the **Surfer SEO** MCP connector. By empowering your LLM to act as a data-driven SEO strategist, you can instantly instantiate new Content Editors, analyze competitors’ prominent NLP terms, and generate full structural audits for any live URL directly from the prompt line. Prevent constant web navigation friction by programmatically evaluating metrics such as precise word counts and real-time Content Scores natively where your content is written.

### What you can do

- **Live Audits & Optimization** — Rapidly inspect published pages analyzing structural deficits utilizing `create_seo_audit` and systematically reviewing results with `get_audit_details`.
- **Content Editor Workflows** — Initiate fresh NLP-guided writing templates invoking `create_content_editor` and fetch essential prominent keywords operating `get_content_editor_details`.
- **Deep SERP Analysis** — Launch statistical data runs commanding `create_serp_analyzer`, evaluating competing structures seamlessly with `get_serp_results` and `get_prominent_terms`.
- **Real-Time Scoring Tests** — Query strict Content Scores across created drafts ensuring structural optimization organically deploying `get_content_score`.

### How it works

1. Append the Surfer SEO MCP module systematically strictly in your integrations control panel.
2. Submit your private `SURFER_KEY` (available via Enterprise or specific plans on Surfer's dashboard) natively to bridge your active account secure authentication.
3. Demand direct operational SEO insights immediately: "Launch a SERP Analyzer querying 'best remote desktop software', and extract its most prominent NLP topics straight to my draft."

### Who is this for?

- **Technical SEO Specialists** — Audit domain performance strictly comparing top-10 competitor matrices avoiding tedious dashboard manual inputs natively in the terminal.
- **Content Managers & Writers** — Orchestrate Content Editor setups structurally bypassing long loading interfaces, extracting target keywords immediately into the conversational flow.
- **Growth Marketers** — Programmatically track Content Scores and generate audits intuitively mapping structural content adjustments logically and safely.


## Available Tools (10)
- **create_seo_audit**: Provide the full URL and target keyword.

Creates a Surfer SEO Audit for a live URL
- **create_content_editor**: Provide a keyword and country code. This is an async operation.

Create a Surfer SEO Content Editor query
- **create_serp_analyzer**: Creates a SERP Analyzer query to identify ranking factors
- **get_audit_details**: Retrieves details for a specific SEO audit
- **get_content_score**: Retrieves the current optimization score for a Content Editor entry
- **get_content_editor_details**: Retrieves Content Editor content and guidelines
- **get_serp_results**: Retrieves SERP Analyzer search results
- **get_prominent_terms**: Retrieves NLP-extracted prominent terms from SERP analysis
- **list_seo_audits**: Lists all SEO audits performed in the account
- **list_content_editors**: Lists all Content Editor queries in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surfer SEO** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the URL 'example.com/blog' using the live API and report the content score alongside any missing prominent keywords."

**🤖 AI Agent:**
> Initiating SEO audit creation ('create_seo_audit') securely... The audit for 'example.com/blog' is processing natively.
Retrieving audit details ('get_audit_details')... 

**Audit Summary Matrix**:
- Current Content Score: 62.
- Top missing NLP terms: 'content marketing strategy', 'organic traffic rationally', 'semantic search implicitly'.

---

**👤 You:**
> "Launch a SERP Analyzer for 'best CRM software' targeting the US market."

**🤖 AI Agent:**
> Commanding NLP engine via `create_serp_analyzer`... Task initiated successfully for 'best CRM software' (United States). The top competitors are currently being mapped. Expect results from `get_serp_results` shortly.

---

**👤 You:**
> "Create a Content Editor draft for the keyword 'how to invest in stocks' with a target score of 75."

**🤖 AI Agent:**
> Creating semantic envelope using `create_content_editor`... Success!
Your Content Editor is ready. Primary NLP terms to include: 'stock market', 'index funds', 'brokerage account'. Hit `get_content_score` as you iterate to verify the 75 baseline.


## ❓ FAQ

**Q: Can the agent natively sequence multiple SERP SEO audits concurrently without degradation?**
Yes. Commands natively hook into asynchronous API creations (like `create_content_editor`). Audits sequence seamlessly provided your API quota from Surfer supports the bulk volume.

**Q: What does the Content Score represent?**
The Content Score is a 0–100 rating generated by Surfer's NLP engine. It measures how well your text covers the prominent terms, word count targets, and structural guidelines extracted from top-ranking pages for your target keyword.

**Q: Which Surfer SEO plan is required for API access?**
API access is available on the Scale AI and Enterprise plans. You can generate your API key from the Surfer dashboard under your account settings once subscribed to an eligible plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surfer-seo](https://vinkius.com/mcp/surfer-seo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surfer SEO** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surfer-seo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surfer SEO** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surfer-seo": {
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
