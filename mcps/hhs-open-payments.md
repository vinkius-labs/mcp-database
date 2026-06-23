# HHS Open Payments MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hhs-open-payments)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Access the HHS Open Payments database to search for physicians, teaching hospitals, and financial relationships in the healthcare industry.

## Description
Connect to the **HHS Open Payments** database to explore financial transparency in healthcare. This server allows you to query datasets, search for specific physicians or teaching hospitals, and analyze payments made by drug and device companies.

### What you can do

- **Dataset Discovery** — List all available Open Payments datasets and inspect their metadata, including column definitions and update timestamps.
- **Physician & Hospital Search** — Search for specific healthcare providers or teaching hospitals by name to find their associated records.
- **Advanced Querying** — Use Socrata Query Language (SoQL) to filter, sort, and limit data for precise financial analysis.
- **Data Export** — Download specific datasets in CSV, JSON, or XML formats for external processing or reporting.
- **Metadata Inspection** — Fetch detailed information about specific datasets to understand the underlying data structure.

### How it works

1. Subscribe to this server
2. Enter your HHS/Socrata API Key (optional but recommended for higher rate limits)
3. Start auditing healthcare financial data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Journalists** — Uncover financial ties between the medical industry and healthcare professionals for investigative reporting.
- **Compliance Officers** — Monitor and verify the accuracy of reported financial transfers within healthcare organizations.
- **Healthcare Consumers** — Check for potential conflicts of interest or financial relationships of their medical providers.


## Available Tools (6)
- **download_dataset**: JSON is recommended for programmatic access.

Download a specific Open Payments dataset
- **get_dataset**: Get metadata for a specific Open Payments dataset
- **list_datasets**: List all available Open Payments datasets
- **query_dataset**: Query specific records within a dataset using SoQL
- **search_hospitals**: Search for specific teaching hospitals
- **search_physicians**: Search for specific physicians


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HHS Open Payments** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available Open Payments datasets."

**🤖 AI Agent:**
> I've retrieved the list of available datasets. There are several active datasets including 'General Payments 2023' (ID: pgaw-6u8r) and 'Research Payments 2023' (ID: 5930-21ab). Which one would you like to explore?

---

**👤 You:**
> "Search for physicians named 'Gregory House' in the database."

**🤖 AI Agent:**
> Searching for 'Gregory House'... I found 2 matching records. One is a specialist in Infectious Diseases in New Jersey. Would you like to see the payment summary for this physician?

---

**👤 You:**
> "Query dataset pgaw-6u8r for payments in Florida where the amount is over $5,000."

**🤖 AI Agent:**
> Executing query on dataset pgaw-6u8r... I found 12 records matching your criteria. The largest payment was $15,400 to a teaching hospital in Miami. Should I list the top 5 results?


## ❓ FAQ

**Q: Can I search for a specific doctor by name to see their financial records?**
Yes! Use the `search_physicians` tool with the doctor's name. The agent will return matching profiles and their associated payment data from the Open Payments database.

**Q: How do I filter data for a specific state or payment amount?**
You can use the `query_dataset` tool and provide a SoQL filter in the `where` parameter (e.g., `recipient_state = 'NY'` or `total_amount_of_payment_usdollars > 1000`).

**Q: What formats can I use to download the datasets?**
The `download_dataset` tool supports 'csv', 'json', and 'xml' formats. JSON is generally recommended for programmatic access and AI analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hhs-open-payments](https://vinkius.com/mcp/hhs-open-payments)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **HHS Open Payments** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hhs-open-payments` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **HHS Open Payments** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hhs-open-payments": {
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
