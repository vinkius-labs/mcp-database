# Ask Kodiak MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ask-kodiak)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance-accounting](../categories/finance-accounting.md)

Search and manage commercial insurance products with Ask Kodiak — track carrier appetite and classifications via AI.

## Description
The **Ask Kodiak MCP Server** brings deep commercial insurance intelligence directly to your AI agent. Effortlessly search for insurance products, monitor carrier appetite, and manage industry classifications (NAICS) using simple natural language.

### Key Features

- **Product Intelligence** — Search across thousands of commercial insurance products based on eligibility, state, and classification.
- **Carrier Oversight** — Access detailed information about insurance companies and their product portfolios.
- **Appetite Matching** — Quickly identify which carriers have an appetite for specific risks or industries.
- **Classification Tools** — Get NAICS code suggestions and search for industry classifications to ensure accurate risk assessment.
- **Real-time Data** — Interface with the Ask Kodiak platform to get the most up-to-date insurance information.
- **Secure API Access** — Uses industry-standard HTTP Basic Authentication with your Group ID and API Key.

### Who is this for?

- **Insurance Brokers** — Instantly find the right products for your clients without manual carrier portal searches.
- **Underwriters** — Audit product details and carrier appetite during your risk evaluation process.
- **Insurtech Developers** — Integrate commercial insurance data retrieval into your automated underwriting workflows.


## Available Tools
- **get_account_check**: Verify Ask Kodiak account connection
- **get_company_products**: List all products offered by a specific company
- **get_product**: Get full appetite and details for an insurance product
- **list_classifications**: Search for industry classifications
- **list_companies**: List insurance carriers and companies
- **list_products**: Search for commercial insurance products
- **suggest_naics**: Get NAICS code suggestions based on a query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ask Kodiak** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List insurance products for NAICS code '541511' in New York."

**🤖 AI Agent:**
> I've retrieved 5 insurance products matching your criteria, including 'Technology Professional Liability' and 'Cyber Risk Protection' from major carriers.

---

**👤 You:**
> "Suggest NAICS codes for a 'Software Development' business."

**🤖 AI Agent:**
> Based on 'Software Development', the top suggestions are: 541511 (Custom Computer Programming Services) and 541512 (Computer Systems Design Services).

---

**👤 You:**
> "Show me all products offered by carrier 'The Hartford'."

**🤖 AI Agent:**
> The Hartford offers 12 commercial products in Ask Kodiak, including General Liability, Workers' Compensation, and Commercial Auto.


## ❓ FAQ

**Q: How do I find my Ask Kodiak Group ID and API Key?**
Log in to your Ask Kodiak account, go to **Company Settings**, and you will find your **Group ID** and **API Key** listed in the API section.

**Q: What is a NAICS code?**
NAICS (North American Industry Classification System) is a standard used by Federal statistical agencies in classifying business establishments for the purpose of collecting, analyzing, and publishing statistical data related to the U.S. business economy.

**Q: Can I search for products by state?**
Yes, use the `list_products` tool and provide the two-letter state code (e.g., 'NY', 'CA') in the `state` parameter to filter results.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ask-kodiak](https://vinkius.com/mcp/ask-kodiak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ask Kodiak** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ask-kodiak` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ask Kodiak** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ask-kodiak": {
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
