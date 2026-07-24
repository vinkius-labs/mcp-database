# Markdown Semantic Chunker Alternative MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-semantic-chunker-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-processing](../categories/data-processing.md)

A deterministic engine for splitting Markdown text into semantically coherent chunks based on header hierarchy and paragraph boundaries.

## Description
The Markdown Semantic Chunker MCP server provides a specialized engine for optimizing Retrieval-Augmented Generation (RAG) pipelines by preserving document structure during the chunking process. Unlike simple character-based splitters that often break sentences or headers mid-way, this tool uses a deterministic approach to identify header levels (# through ######) and group content accordingly. By maintaining a hierarchical path for every chunk, such as Intro > Setup > Step 1, it ensures that downstream LLMs receive the full structural context of each text segment. When a section exceeds the user-defined maxChunkSizeTokens, the engine intelligently splits at paragraph boundaries (double newlines) to maintain semantic integrity. The server includes specialized tools like generate_semantic_chunks for primary execution, get_header_structure for hierarchy previews, and calculate_markdown_token_density for analyzing text density.


## Available Tools (3)
- **generate_semantic_chunks**: Generates semantic chunks from markdown content
- **get_header_structure**: Extracts the header structure from markdown
- **calculate_markdown_token_density**: Calculates the token density of markdown content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markdown Semantic Chunker Alternative** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split this markdown text into chunks with a maximum of 100 tokens: # Introduction
This is the intro.
## Setup
Step 1: Install dependencies."

**🤖 AI Agent:**
> The text was split into two chunks. Chunk 1: 'Introduction - This is the intro.' (Path: Introduction). Chunk 2: 'Setup - Step 1: Install dependencies.' (Path: Introduction > Setup).

---

**👤 You:**
> "Analyze the token density of this markdown block."

**🤖 AI Agent:**
> The analysis shows 2 distinct paragraphs and an estimated total of 45 tokens for the provided text block.

---

**👤 You:**
> "Show me all the headers in this document: # Title
## Section A
### Sub-section 1"

**🤖 AI Agent:**
> The detected hierarchy is: ['Title', 'Title > Section A', 'Title > Section A > Sub-section 1'].


## ❓ FAQ

**Q: How does the chunking process maintain context?**
The tool assigns a hierarchical path to every chunk, representing its position in the document tree (e.g., Parent > Child). This ensures that even when text is split, the structural lineage remains attached to the content.

**Q: What happens if a section is too large for the token limit?**
If a header group exceeds the maxChunkSizeTokens, the engine identifies paragraph boundaries marked by double newlines and splits the content at these points to create smaller, valid chunks.

**Q: Can I preview the document structure before chunking?**
Yes, you can use the get_header_structure tool to extract and view the identified heading hierarchy without performing the full chunking operation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-semantic-chunker-alternative](https://vinkius.com/mcp/markdown-semantic-chunker-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Markdown Semantic Chunker Alternative** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `markdown-semantic-chunker-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Markdown Semantic Chunker Alternative** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "markdown-semantic-chunker-alternative": {
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
