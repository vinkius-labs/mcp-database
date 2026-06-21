# DocBreach MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/docbreach)
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


## Available Tools (5)
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


## ❓ FAQ

**Q: How does DocBreach bypass modern Single Page Application (SPA) barriers?**
DocBreach features a built-in hydration engine. Rather than relying on a heavy headless browser, it intercepts and evaluates underlying framework payloads (like `__NEXT_DATA__` for Next.js or Docusaurus state) to extract the raw documentation text directly. This makes it blisteringly fast and resource-efficient.

**Q: What documentation formats and frameworks are officially supported?**
It natively parses OpenAPI/Swagger specifications, Postman Collections, and standard `llms.txt` files. For web-based docs, it surgically cleans noise from 12+ major frameworks including Docusaurus, Nextra, VitePress, Mintlify, GitBook, and ReadMe, returning LLM-optimized Markdown.

**Q: Do I need any third-party API keys or paid scraping subscriptions?**
Absolutely not. DocBreach is designed to operate completely independently. It accesses public documentation directly via optimized HTTP clients using smart resolution strategies, eliminating the need for proxy services, SaaS subscriptions, or scraping API keys.

**Q: How does this MCP server improve my AI Agent's performance?**
AI Agents typically hallucinate when APIs are updated or when facing undocumented endpoints. By equipping your agent with DocBreach, it can autonomously search, map, and read the definitive, up-to-date source of truth before writing a single line of code, ensuring deterministic integrations.

**Q: Can it extract specific endpoints from massive OpenAPI specifications?**
Yes! The `docs.extract` tool is built precisely for this. Instead of loading a 5MB JSON spec into your agent's context window (which wastes tokens and ruins attention), DocBreach parses the spec server-side and allows your agent to query exactly the endpoints and methods it needs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docbreach](https://vinkius.com/mcp/docbreach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DocBreach** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `docbreach` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DocBreach** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "docbreach": {
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
