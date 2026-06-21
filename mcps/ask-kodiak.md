# Ask Kodiak MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ask-kodiak)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ask-kodiak-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ask-kodiak-mcp)
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


## Installation & Usage

To install and use the **Ask Kodiak** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ask-kodiak](https://vinkius.com/mcp/ask-kodiak)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
