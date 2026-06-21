# Smithsonian Open Access MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smithsonian-open-access)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore millions of museum records, images, and digital assets from the Smithsonian Institution's vast collections.

## Description
Connect to the **Smithsonian Open Access** repository and bring millions of museum records, scientific data, and historical artifacts directly into your AI workspace. This server provides programmatic access to the Smithsonian's Enterprise Digital Asset Network (EDAN).

### What you can do

- **Global Search** — Query millions of records across all Smithsonian units using the `search_records` tool to find images, specimens, and artifacts.
- **Detailed Metadata** — Use `get_content` to retrieve comprehensive descriptions, provenance, and digital asset links for specific museum objects.
- **Categorized Discovery** — Narrow your research to specific fields like art, history, or science using the `search_category` tool for more precise results.
- **Research & Education** — Instantly pull primary source data for academic research, educational content, or creative projects.

### How it works

1. Subscribe to this server
2. Enter your Smithsonian API Key
3. Start exploring the world's largest museum, education, and research complex through Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Academics** — quickly gather metadata and primary source information for scholarly work
- **Educators** — find high-quality museum records and images to enhance learning materials
- **Developers & Creatives** — integrate authentic historical and scientific data into applications and digital experiences


## Available Tools (3)
- **search_category**: Search within specific categories or units
- **get_content**: Retrieve a specific museum record by its unique identifier
- **search_records**: Search for museum records across all Smithsonian units


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Smithsonian Open Access** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for records related to the Apollo 11 mission."

**🤖 AI Agent:**
> I've found several records for the Apollo 11 mission, including the Command Module 'Columbia', lunar samples, and commemorative medals. Would you like the details for any of these items?

---

**👤 You:**
> "Get the full details for the record with ID edanmdm:nmah_1313964."

**🤖 AI Agent:**
> I've retrieved the metadata for ID edanmdm:nmah_1313964. This record corresponds to the 'Star-Spangled Banner', the flag that inspired the U.S. national anthem, currently held at the National Museum of American History.

---

**👤 You:**
> "Search for 'impressionism' within the art category."

**🤖 AI Agent:**
> Searching for 'impressionism' in the art category... I found works by Mary Cassatt, John Singer Sargent, and various French impressionist prints. Which artist or specific work should we explore?


## ❓ FAQ

**Q: Can I search for specific historical figures across all Smithsonian museums?**
Yes! Use the `search_records` tool with your query (e.g., 'Abraham Lincoln'). It will return matching records, images, and artifacts from across all Smithsonian units.

**Q: How do I get the full metadata for a specific museum object?**
Use the `get_content` tool with the unique identifier (ID) of the record. This will fetch detailed metadata, including descriptions, dates, and media links.

**Q: Is it possible to limit my search to just art or science categories?**
Yes, the `search_category` tool allows you to specify a category (like 'art', 'history', or 'science') along with your search query to get more targeted results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smithsonian-open-access](https://vinkius.com/mcp/smithsonian-open-access)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Smithsonian Open Access** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smithsonian-open-access` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Smithsonian Open Access** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smithsonian-open-access": {
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
