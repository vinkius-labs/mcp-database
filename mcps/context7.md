# Context7 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/context7)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/context7-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/context7-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [friends-mcp](../categories/friends-mcp.md)

Empower AI agents via Context7 — pull up-to-date documentation and code examples for any library or framework directly into your workspace.

## Description
Connect your **Context7** account to any AI agent and provide it with the most up-to-date, version-specific technical documentation through natural conversation.

### What you can do

- **Library Discovery** — Resolve fuzzy framework names (e.g., 'react', 'tailwind') into deterministic paths and specific versions needed for accurate documentation
- **Live Docs Querying** — Analyze specific localized variables and retrieve raw Markdown documentation chunks to ground your agent in technical truths
- **Code Example Extraction** — Pull valid, version-specific code examples for any component or function directly into your development flow
- **RAG for Developers** — Use Context7 as a documentation-specialized RAG layer to ensure your agent never hallucinates outdated API signatures
- **Up-to-date Knowledge** — Access documentation that is synchronized with the latest releases, bypassing the training cutoff limits of standard LLMs

### How it works

1. Subscribe to this server
2. Enter your Context7 API Key (found in your Context7/Upstash Dashboard)
3. Start querying technical documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — pull specific API documentation and code snippets without leaving the IDE or searching manually
- **AI Engineers** — ground coding agents in real-time technical documentation to improve code generation accuracy
- **Technical Writers** — verify version-specific API signatures and cross-reference documentation blocks quickly
- **Rapid Prototypers** — instantly retrieve boilerplates and component examples for new frameworks and libraries


## Available Tools
- **resolve_library**: g. react) into deterministic paths (e.g. /facebook/react/18.2.0) needed for deep documentation fetching.

Find the correct exact library ID and latest version matching a framework or library search query
- **query_docs**: Query documentation and code examples for a specific library ID (from resolve_library tool) about a certain topic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Context7** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Resolve the library ID for 'nextjs'"

**🤖 AI Agent:**
> I've resolved 'nextjs' to the following IDs: 'vercel/next.js/14.1.0' (latest), 'vercel/next.js/13.5.6', and 'vercel/next.js/12.3.4'. Which version would you like to query documentation for?

---

**👤 You:**
> "Show me how to use 'App Router' in Next.js 14"

**🤖 AI Agent:**
> Retrieving documentation for 'App Router' in Next.js 14.1.0... [Agent pulls official Markdown segments detailing layout.js and page.js structure with code examples].

---

**👤 You:**
> "What are the new features in Tailwind CSS v4?"

**🤖 AI Agent:**
> Querying Tailwind CSS v4.0.0 docs... The main updates include the new high-performance engine, native CSS variables support, and simplified configuration. I can provide the exact code examples for these new features.


## Installation & Usage

To install and use the **Context7** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/context7](https://vinkius.com/mcp/context7)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
