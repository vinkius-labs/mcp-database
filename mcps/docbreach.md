# DocBreach MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docbreach)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/docbreach-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/docbreach-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Real-time documentation discovery for AI agents. Discover, read, and extract any API documentation without browser rendering or API keys.

## Description
The web is hostile to AI agents. DocBreach brings a crowbar. Discover, read, and extract any API documentation in real-time — without browser rendering, without API keys, without SaaS dependencies. Supports OpenAPI, Swagger, Postman Collections, llms.txt, and 12+ SPA frameworks.

### What you can do

- **Discover Sources** — Find documentation sources for any service or API using `docs.discover`.
- **Read Documentation** — Read any documentation URL and return clean, LLM-ready Markdown using `docs.read`.
- **Map Structures** — Map the complete documentation structure of any domain via sitemaps using `docs.map`.
- **Search Topics** — Search for specific topics within a documentation site using `docs.search`.
- **Extract Endpoints** — Extract structured endpoint information from OpenAPI specs using `docs.extract`.

### How it works

1. Subscribe to this server
2. No authentication is required
3. Start using the tools to read and extract documentation directly from your AI agent

### Who is this for?

- **Developers** — Find API documentation for code generation and read library documentation during coding sessions.
- **AI Agents** — Extract API endpoints from OpenAPI specifications and map entire documentation sites for comprehensive context.


## Available Tools
- **docs_search**: Always provide the "site" parameter when searching within a known domain. Example: docs.search({ query: "authentication headers", site: "docs.stripe.com" })

Search for specific topics within a documentation site
- **docs_discover**: Use specific, descriptive queries. Example: "stripe API webhooks" instead of just "stripe". Combine your search intents into a single query. Do NOT call this tool in rapid loops — refine your query instead.

Find documentation sources for any service, library, or API
- **docs_map**: Provide a domain (e.g., "stripe.com") and receive a complete table of contents with every documentation page organized by section. Then use docs.read on specific pages from the map.

Map the complete documentation structure of any domain
- **docs_read**: Handles HTML, JSON, YAML, OpenAPI specs, Postman Collections, PDFs (<5MB), and llms.txt. The response includes a "Related Documentation Links" section extracted from page navigation. ALWAYS check these links for authentication and getting-started pages before generating code.

Read any documentation URL and return clean, LLM-ready Markdown
- **docs_extract**: read has identified an OpenAPI/Swagger spec URL or Postman Collection. Provide a tag to filter endpoints by API group. If no tag is provided, returns a summary of all tags with endpoint counts.

Extract structured endpoint information from an OpenAPI, Swagger, or Postman spec


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DocBreach** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the official integration guide for Stripe webhooks and read the first steps."

**🤖 AI Agent:**
> I've reviewed the Stripe Webhooks documentation at `https://docs.stripe.com/webhooks`. The guide outlines 3 main steps to listen for events: setting up an endpoint, parsing the payload, and verifying signatures. Would you like me to generate the implementation code based on this guide?

---

**👤 You:**
> "Extract all the user authentication endpoints from the GitHub REST API specification."

**🤖 AI Agent:**
> I've analyzed the GitHub OpenAPI spec and found 5 endpoints related to user authentication under the 'users' tag. The primary endpoints are `GET /user` for the authenticated user and `PATCH /user` to update the profile. Which endpoint would you like to see the required parameters for?

---

**👤 You:**
> "Map the documentation structure for Vercel's v0 to see all available topics."

**🤖 AI Agent:**
> I've mapped the documentation for `v0.dev`. There are 42 pages in total, structured under 'Concepts', 'UI Components', and 'Billing'. The most relevant page for getting started seems to be `https://v0.dev/docs/introduction`. Shall I read that page for you?

---

**👤 You:**
> "Search the Next.js documentation for how to implement Server Actions."

**🤖 AI Agent:**
> Based on the Next.js documentation, specifically the 'Data Fetching: Server Actions and Mutations' guide, you implement Server Actions using the `"use server"` directive. Should I output the code example for a basic form mutation?

---

**👤 You:**
> "Read the React 19 documentation on the useActionState hook and summarize its return values."

**🤖 AI Agent:**
> According to the React 19 documentation, `useActionState` returns an array with three values: `[state, formAction, isPending]`. The `isPending` boolean is new and replaces the need for `useFormStatus` in many cases. Do you want to see a full implementation example?


## Installation & Usage

To install and use the **DocBreach** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docbreach](https://vinkius.com/mcp/docbreach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
