# Namsor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/namsor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Automate name analytics via Namsor — predict gender, origin, and ethnicity directly from any AI agent.

## Description
Connect your **Namsor** account to any AI agent and simplify your name analytics and demographic enrichment through natural conversation.

### What you can do

- **Gender Prediction** — Analyze first and last names to determine gender with high accuracy and probability metrics
- **Origin & Residency** — Predict a name's country of origin and likely current country of residency
- **Ethnicity Tracking** — Query US-specific ethnicity models (Hispanic, Asian, Black, White) for localized demographic insights
- **Name Parsing** — Break down complex full name strings into structured components (prefix, first, last, suffix)
- **Diaspora Insights** — Predict the diaspora group or ethnic cluster for a name within a specific country context

### How it works

1. Subscribe to this server
2. Enter your Namsor API v2 Key from your account dashboard
3. Start enriching your lead and customer data from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **predict_country**: Predict country residency from name
- **predict_diaspora**: Predict diaspora from name
- **predict_ethnicity**: g., Hispanic, Asian, White).

Predict US ethnicity from name
- **predict_gender**: Predict gender from name
- **predict_origin**: Predict country of origin from name
- **parse_full_name**: Parse a full name string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Namsor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the gender for the name 'Jean Dupont'."

**🤖 AI Agent:**
> Based on Namsor analytics, 'Jean Dupont' is predicted as Male with 98% probability in France.

---

**👤 You:**
> "What is the likely country of origin for the name Yuki Tanaka?"

**🤖 AI Agent:**
> Based on onomastic analysis, the name Yuki Tanaka has a 97.2% probability of Japanese origin. The top region match is East Asia with strong confidence in the JP country code.

---

**👤 You:**
> "Parse the full name Dr. Maria Elena Rodriguez-Garcia into its components."

**🤖 AI Agent:**
> I parsed the name successfully. Title: Dr., First Name: Maria Elena, Last Name: Rodriguez-Garcia. The name structure suggests a Hispanic compound surname pattern with a professional prefix.


## ❓ FAQ

**Q: Can I predict gender using only a name?**
Yes! Use the `predict_gender` tool. Provide the first and last name, and the agent will return the most likely gender and its probability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/namsor](https://vinkius.com/mcp/namsor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Namsor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `namsor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Namsor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "namsor": {
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
