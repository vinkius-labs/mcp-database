# Cannlytics Strain API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cannlytics-strain-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access cannabis strain data, effects, flavors, and similar strains via Cannlytics.

## Description
Connect **Cannlytics** to any AI agent and access structured, open cannabis strain data -- search strains, view effects and flavors, and discover similar strains through natural conversation.

### What you can do
- **Strain Search** -- Find cannabis strains by name or keyword
- **Effects & Flavors** -- Retrieve detailed positive, negative, and medical effects plus flavor profiles
- **Similar Strains** -- Discover related strains based on genetics or characteristics

### How it works
1. Subscribe to this server
2. Enter your Cannlytics API Key
3. Start exploring cannabis data from Claude, Cursor, or any MCP-compatible client

Cannlytics provides an open API for transparent cannabis data, serving consumers, researchers, and industry professionals.

### Who is this for?
- **Consumers** -- Verify strain effects and flavors before making a purchase
- **Budtenders** -- Quickly find similar strains and medical benefits to guide customers
- **Researchers** -- Access structured cannabis data for studies and market analysis


## Available Tools
- **get_effects**: Get reported effects for a specific strain
- **get_flavors**: g., earthy, sweet, citrus) for the strain.

Get flavor profile for a specific strain
- **get_strain**: Get detailed information for a specific cannabis strain
- **search_strains**: Use this to discover available strains in the Cannlytics database.

Search for cannabis strains by name or keyword
- **get_similar_strains**: Find strains similar to a specific strain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cannlytics Strain API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for strains with 'Blue' in the name."

**🤖 AI Agent:**
> Found 5 strains: 1. Blue Dream. 2. Blueberry. 3. Blue Cheese. 4. Blue Cookies.

---

**👤 You:**
> "What are the effects of Sour Diesel?"

**🤖 AI Agent:**
> Effects: Energetic, Uplifted, Creative (Positive). Dry Mouth, Anxious (Negative). Stress, Pain (Medical).

---

**👤 You:**
> "Show me strains similar to OG Kush."

**🤖 AI Agent:**
> Similar strains: 1. Skywalker OG. 2. Bubba Kush. 3. Master Kush.


## ❓ FAQ

**Q: How do I get my Cannlytics API Key?**
Sign up on the Cannlytics platform, navigate to your account settings, and generate a new API key.

**Q: Can I see medical effects for strains?**
Yes, the get_effects tool returns positive, negative, and medical effects reported by users for each strain.

**Q: Does it include flavor profiles?**
Yes, use the get_flavors tool to see detailed flavor descriptors like earthy, sweet, citrus, and more.

**Q: Can I find similar strains to one I already know?**
Yes! Use the get_similar_strains tool to discover related strains based on genetics and shared characteristics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cannlytics-strain-api](https://vinkius.com/mcp/cannlytics-strain-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cannlytics Strain API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cannlytics-strain-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cannlytics Strain API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cannlytics-strain-api": {
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
