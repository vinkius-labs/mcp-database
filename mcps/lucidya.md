# Lucidya MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lucidya)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Monitor social media, analyze sentiment, and manage customer data via the Lucidya API.

## Description
Connect your **Lucidya** account to any AI agent to automate your social listening and customer engineering intelligence. This MCP server enables your agent to list monitors, analyze text sentiment using advanced AI, and retrieve unified customer profiles directly from natural language interfaces.

### What you can do

- **Social Listening** — List all active and inactive monitors across Twitter, Instagram, and other sources
- **AI Analysis** — Perform advanced sentiment analysis and Arabic dialect detection on any text string
- **CDP Access** — Retrieve unified customer profiles and interaction histories from the Lucidya Customer Data Platform
- **Service Analytics** — Query KPIs and performance metrics for customer service via the OmniServe API
- **Real-time Monitoring** — Fetch complete metadata and status for your configured listening monitors

### How it works

1. Subscribe to this server
2. Enter your Lucidya API Token
3. Start managing your social intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Brand Managers** — Monitor social mentions and brand sentiment via simple natural language commands
- **Customer Experience Teams** — Quickly retrieve unified customer profiles and interaction histories
- **Data Analysts** — Automate the extraction of social metrics and AI-driven sentiment logs into your workflow


## Available Tools (7)
- **list_cdp_customers**: List customer profiles from CDP
- **detect_arabic_dialect**: Detect the specific Arabic dialect of a text
- **get_customer_profile**: Get complete details for a customer profile
- **get_monitor_details**: Get details for a specific monitor
- **list_social_monitors**: List all social media monitors
- **analyze_text_sentiment**: Analyze the sentiment of a given text
- **get_omniserve_analytics**: Query customer service analytics KPIs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lucidya** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my social media monitors in Lucidya."

**🤖 AI Agent:**
> I've retrieved your monitors. You have 5 active monitors, including 'Competitor Tracking', 'Brand Mentions', and 'Campaign Launch 2024'.

---

**👤 You:**
> "Analyze the sentiment of this text: 'I am extremely happy with the new product release!'."

**🤖 AI Agent:**
> The AI analysis confirms a 🟢 Positive sentiment for that text, with a high confidence score of 0.98.

---

**👤 You:**
> "Show the customer profile for ID 'cust-123' in the Lucidya CDP."

**🤖 AI Agent:**
> I've fetched the profile for customer cust-123. They have interact with your brand 12 times across Twitter and Intercom, with an overall sentiment score of 0.85 (Neutral-Positive).


## ❓ FAQ

**Q: How do I find my API Token?**
Log in to your Lucidya account and navigate to Account Settings or API section to generate and copy your unique authorization token.

**Q: Does the AI analysis work for languages other than English?**
Yes, Lucidya's AI is highly optimized for multiple languages, with specific advanced support for various Arabic dialects.

**Q: Can I retrieve historical social data?**
You can retrieve any data that has been captured by your active monitors. Use the `monitor_details` tool to check what is currently being monitored.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lucidya](https://vinkius.com/mcp/lucidya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lucidya** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lucidya` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lucidya** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lucidya": {
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
