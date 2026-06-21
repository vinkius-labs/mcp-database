# Google Fonts API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-fonts-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage web fonts — audit families, variants, and categories via AI.

## Description
Empower your AI agent to orchestrate your entire visual design and font auditing workflow with the **Google Fonts API**, the world's most popular source for open-source typography. By connecting Google Fonts to your agent, you transform complex font searches into a natural conversation. Your agent can instantly search for thousands of font families, audit available variants and subsets, and identify trending styles without you ever touching a design portal. Whether you are building brand guidelines or conducting typographic research, your agent acts as a real-time design consultant, ensuring your typography is always expressive and technically precise.

### What you can do

- **Font Auditing** — Retrieve high-resolution metadata for any font family in the Google catalog, including categories and update history.
- **Variant Oversight** — Audit the available weights and styles for specific fonts to maintain a clear view of typographic versatility.
- **Trend Discovery** — Query fonts sorted by popularity or trending status to understand current industry leads in web typography.
- **Subset Intelligence** — Identify supported language subsets for any font to assist in regional and international design planning.
- **Operational Monitoring** — Check API status to ensure your design research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Google Cloud API Key
3. Start managing your typographic intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Designers & Creatives** — monitor font trends and retrieve high-quality metadata straight from your workflow.
- **Developers** — verify font availability and audit variant distributions without manual searching.
- **Marketing Teams** — perform rapid audits of typography for brand consistency and identify relevant styles through natural language.
- **Operations Leads** — automate design data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **check_api_status**: Check if the Google Fonts service is operational
- **get_font_details**: Get full metadata and variants for a specific font family
- **list_all_fonts**: List all fonts available in the Google Fonts catalog
- **search_fonts**: Search for fonts by family name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Fonts API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for font family 'Roboto' using Google Fonts API."

**🤖 AI Agent:**
> I've retrieved the details for Roboto! It belongs to the 'sans-serif' category and has 12 variants, ranging from '100' to '900 italic'. Would you like the full list of supported subsets for this font?

---

**👤 You:**
> "Show the top 5 most popular fonts on Google Fonts."

**🤖 AI Agent:**
> I've identified the 5 most popular font families! They include Roboto, Open Sans, Lato, Montserrat, and Oswald. I can provide the category and variant metadata for each of these if you'd like.

---

**👤 You:**
> "What fonts were recently modified?"

**🤖 AI Agent:**
> I've retrieved the list of recently updated fonts! Notable entries include [Font Name] and [Font Name], both modified in the last 30 days. I can assist you with an audit of the new variants or styles for these families.


## ❓ FAQ

**Q: How do I find my Google Fonts API Key?**
Log in to the [**Google Cloud Console**](https://console.cloud.google.com/), enable the 'Google Fonts Developer API', and create an API Key in the 'Credentials' section. Copy and paste it below.

**Q: Can I sort fonts by popularity?**
Yes. Use the `list_all_fonts` tool and provide the `sort` parameter as 'popularity'. Your agent will return the most widely used fonts first.

**Q: Are available weights included in the details?**
Yes. Every font family record retrieved by your agent includes a full list of available variants (e.g., 'regular', '700', 'italic') and supported subsets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-fonts-api](https://vinkius.com/mcp/google-fonts-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Fonts API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `google-fonts-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Fonts API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-fonts-api": {
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
