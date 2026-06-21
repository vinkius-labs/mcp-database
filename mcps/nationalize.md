# Nationalize MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nationalize)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Predict the nationality of a person based on their name using the Nationalize.io API.

## Description
The **Nationalize** MCP server allows your AI agent to estimate the most likely country of origin for any given name. By analyzing linguistic patterns and global data, it provides a ranked list of ISO country codes and probability scores.

### What you can do

- **Nationality Prediction** — Submit up to 10 names at once to receive statistical predictions about their origin.
- **Data Enrichment** — Enhance user profiles or lead data with probable geographic context.
- **Global Insights** — Understand the demographic distribution of names within your datasets.

### How it works

1. Subscribe to this server
2. Enter your Nationalize.io API Key (optional for low-volume testing)
3. Start predicting origins from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — Quickly categorize large lists of names by probable region.
- **Developers** — Integrate demographic estimation into applications without building complex models.
- **Researchers** — Analyze naming trends and geographic distributions across different cultures.


## Available Tools
- **predict_nationality**: Best results are achieved by sending the last name.

Predict the nationality of a person based on their name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nationalize** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the nationality for the name 'Dmitry'."

**🤖 AI Agent:**
> I've analyzed the name 'Dmitry'. The most likely country of origin is Russia (RU) with a probability of 0.15, followed by Ukraine (UA) and Belarus (BY).

---

**👤 You:**
> "What are the most likely countries of origin for 'Silva' and 'Tanaka'?"

**🤖 AI Agent:**
> For 'Silva', the top prediction is Brazil (BR) with high confidence. For 'Tanaka', the most likely origin is Japan (JP). Would you like the full probability breakdown for both?

---

**👤 You:**
> "Check the origin of the last name 'O'Connor'."

**🤖 AI Agent:**
> The name 'O'Connor' shows a very strong correlation with Ireland (IE) at 0.92 probability. Other minor matches include the United Kingdom and Australia.


## ❓ FAQ

**Q: How many names can I analyze in a single request?**
You can pass a list of up to 10 names to the `predict_nationality` tool per request. This allows for efficient batch processing of datasets.

**Q: What kind of results does the tool return?**
The tool returns a ranked list of ISO 3166-1 alpha-2 country codes (like 'US', 'BR', 'JP') along with a probability score for each, indicating the likelihood of that origin.

**Q: Is an API key required to use this server?**
The `NATIONALIZE_API_KEY` is optional. You can perform basic testing without it, but for higher volume or production use, providing a key is recommended to avoid rate limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nationalize](https://vinkius.com/mcp/nationalize)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nationalize** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nationalize` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nationalize** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nationalize": {
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
