# Surfer SEO MCP Server

Connect your AI to Surfer SEO. Generate Content Editors, perform NLP SERP audits, and extract high-ranking keyword guidelines directly from the terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/surfer-seo)

## Overview
**Category:** marketing-automation
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Surfer SEO** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/surfer-seo](https://vinkius.com/mcp/surfer-seo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
