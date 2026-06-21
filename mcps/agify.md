# Agify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Predict the age of a person based on their first name using the Agify.io API.

## Description
Connect your AI agent to **Agify.io** to instantly estimate the age of individuals or groups based on their first names. This server provides powerful demographic intelligence for data enrichment and user profiling.

### What you can do

- **Individual Prediction** — Estimate the age of a single person by providing their first name.
- **Country Scoping** — Improve accuracy by narrowing the prediction to a specific country using ISO codes.
- **Batch Processing** — Predict ages for up to 10 names in a single request for efficient data analysis.
- **Probability Metrics** — Receive not just an age, but the data count used to generate the prediction.

### How it works

1. Subscribe to this server
2. Enter your Agify API Key (optional for limited testing)
3. Start predicting demographics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — Enrich user databases with estimated demographic information.
- **Marketing Teams** — Segment leads and audiences based on name-derived age estimates.
- **Developers** — Build smarter onboarding flows or personalization engines without asking for birth dates.


## Available Tools
- **predict_age_batch**: Predict the ages of multiple people based on their first names
- **predict_age**: Optionally scope by country.

Predict the age of a person based on their first name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the age for the name 'Michael'."

**🤖 AI Agent:**
> Based on the Agify database, the estimated age for 'Michael' is 44 years old (based on 233,482 data points).

---

**👤 You:**
> "What is the estimated age for 'Isabella' in Italy (IT)?"

**🤖 AI Agent:**
> In Italy, the name 'Isabella' has an estimated age of 52 years.

---

**👤 You:**
> "Predict the ages for these names: 'John', 'Emma', and 'Liam'."

**🤖 AI Agent:**
> I've processed the batch: 'John' is estimated at 51, 'Emma' at 34, and 'Liam' at 21.


## ❓ FAQ

**Q: Can I predict the age of multiple people at once?**
Yes! Use the `predict_age_batch` tool. You can provide an array of up to 10 names in a single request to get multiple age estimations efficiently.

**Q: How can I make the age prediction more accurate for a specific region?**
When using the `predict_age` tool, you can provide an optional `country_id` (ISO 3166-1 alpha-2 code). This scopes the data to that specific country, providing a more localized age estimate.

**Q: Is an API key required to use this server?**
An API key is optional for low-volume testing, but recommended for production use or higher rate limits. You can obtain one at Agify.io.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agify](https://vinkius.com/mcp/agify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `agify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agify": {
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
