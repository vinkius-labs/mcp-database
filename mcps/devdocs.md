# DevDocs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/devdocs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Search and read developer documentation via DevDocs.io — list libraries, find specific API pages, and retrieve Markdown docs directly from any AI agent.

## Description
Connect your AI agent to the **DevDocs.io** index and take full control of your technical documentation research and coding assistance through natural conversation.

### What you can do

- **Library Discovery** — List all supported programming languages, frameworks, and SDKs (e.g., AWS, Vue 3, Rust) available in the DevDocs global registry
- **Documentation Indexing** — Directly query internal search indexes matching strict component or class names to find exact manual page paths
- **Knowledge Retrieval** — Fetch explicitly tracked payload URLs and translate native static HTML blobs directly into clean, human-readable Markdown
- **SDK Oversight** — Identify available SDK library definitions and verify precise versioning boundaries ready for offline reading and agent grounding
- **Contextual Code Assistance** — Pull valid, version-specific documentation chunks to provide high-quality technical context for your development tasks

### How it works

1. Subscribe to this server
2. No credentials required — this server uses the public DevDocs.io registry
3. Start querying technical documentation from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Developers** — search for specific API references and documentation without leaving the IDE or browser
- **AI Engineers** — ground coding agents in real-time technical documentation to improve the quality of generated code
- **Technical Writers** — verify API signatures and cross-reference documentation blocks across multiple frameworks
- **Polyglot Programmers** — quickly navigate documentation for different languages and tools using a unified search interface


## Available Tools
- **list_libraries**: List all supported programming languages, frameworks, and SDKs (e.g. aws, vue~3, rust) available in DevDocs
- **search_docs**: Search the index of a specific documentation library to find the exact manual page path
- **read_page**: Read the content of a specific documentation page. Returns cleanly formatted Markdown text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DevDocs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all documentation libraries available in DevDocs"

**🤖 AI Agent:**
> I've retrieved the full list of libraries. You can search documentation for hundreds of tools including 'aws', 'docker', 'git', 'javascript', 'nextjs', 'react', 'rust', and 'tailwindcss'. Which one would you like to explore?

---

**👤 You:**
> "Search for 'useState' in the react documentation"

**🤖 AI Agent:**
> Searching react index for 'useState'... I found the exact page path: 'hooks-state.html'. I can pull the full Markdown documentation and code examples for you.

---

**👤 You:**
> "Read the documentation for 'aws' at path 'cli/s3/cp'"

**🤖 AI Agent:**
> Retrieving 'aws' documentation for 's3 cp'... [Agent pulls official Markdown segments detailing the cp command, including description, usage syntax, and examples like 'aws s3 cp file.txt s3://my-bucket/'].


## ❓ FAQ

**Q: Does this server require a DevDocs.io account or API key?**
No. This server uses the public DevDocs.io registry and documentation indices, which do not require authentication. You can start querying technical documentation immediately without any setup.

**Q: Can my agent search within a specific library like 'react' or 'tailwindcss'?**
Yes. Use the 'search_docs' tool. Provide the library slug (e.g., 'react') and your search query. The agent will directly attack the internal search index, rapidly filtering available paths matching your keyword.

**Q: How do I get the actual documentation content in Markdown format?**
Use the 'read_page' tool. Provide the library slug and the exact page path (which you can find using search_docs). Your agent will translate the native DevDocs static HTML blobs directly into clean, human-readable Markdown payloads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/devdocs](https://vinkius.com/mcp/devdocs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DevDocs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `devdocs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DevDocs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "devdocs": {
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
