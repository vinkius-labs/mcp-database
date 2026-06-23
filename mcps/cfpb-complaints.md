# CFPB Complaints MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cfpb-complaints)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search 13.8M+ consumer complaints against financial companies — filter by product, company, state and issue.

## Description
Connect to **CFPB Consumer Complaint Database** and explore 13.8M+ consumer complaints through natural conversation — no API key needed.

### What you can do

- **Complaint Search** — Search complaints by product, company, state, issue and date range
- **Company Complaints** — View all complaints against a specific company
- **State Complaints** — Browse complaints from a specific US state
- **Product Complaints** — Find complaints for specific financial products (Mortgage, Debt Collection, Credit Card)
- **Consumer Narratives** — Read detailed consumer narratives describing their experiences
- **Recent Complaints** — Track recently filed complaints and complaint trends
- **Statistics** — Get complaint counts for quick analysis

### How it works

1. Subscribe to this server
2. No API key needed — data is open public domain
3. Start exploring complaint data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Consumers** — research company complaint histories before choosing financial products
- **Researchers** — analyze complaint trends, company responses and regulatory patterns
- **Journalists** — find complaint data for investigative reporting on financial companies


## Available Tools (9)
- **get_company_complaints**: Returns complaint details including products, issues, states, dates and company responses.

Get complaints against a specific company
- **get_complaint**: Returns full complaint details including product, company, issue, narrative (if available), dates and company response.

Get a specific complaint by ID
- **get_complaints_by_issue**: Common issues: "Incorrect information", "Problem with a purchase", "Attempts to collect debt not owed".

Get complaints for a specific issue type
- **get_complaints_by_product**: Common products: "Mortgage", "Debt collection", "Credit card", "Student loan", "Credit reporting".

Get complaints for a specific product type
- **get_complaints_by_state**: Returns complaint details including products, companies, issues and dates.

Get complaints from a specific US state
- **get_complaints_stats**: Useful for getting a quick count without retrieving full complaint details.

Get complaint count statistics
- **get_complaints_with_narrative**: Supports filtering by product, company and state.

Get complaints that include consumer narratives (detailed descriptions)
- **get_recent_complaints**: Useful for tracking recent complaint trends.

Get the most recent consumer complaints
- **search_complaints**: 8M+ complaints against financial companies. Supports filtering by product, company, state, issue, date range and narrative availability. Returns complaint details including product type, company name, issue, state, date received and company response.

Search consumer complaints in the CFPB database


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CFPB Complaints** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me recent complaints about Wells Fargo."

**🤖 AI Agent:**
> Found 15 recent complaints against Wells Fargo covering: Mortgage (incorrect information), Credit card (unauthorized charges), Bank account (unexpected fees). Companies responded to 80% of complaints.

---

**👤 You:**
> "What are the most common issues with debt collection?"

**🤖 AI Agent:**
> Top debt collection issues: Attempts to collect debt not owed (35%), Continued collection after dispute (22%), Incorrect information on credit report (18%), Harassment (15%), False statements (10%).

---

**👤 You:**
> "How many complaints does Equifax have?"

**🤖 AI Agent:**
> Equifax has 350,000+ complaints in the database. Top issues: Incorrect information (45%), Problem with credit report (30%), Unable to get credit report (15%). Most common product: Credit reporting.


## ❓ FAQ

**Q: Do I need an API key?**
No! CFPB complaint data is completely free and open public domain. No authentication required.

**Q: What products are covered?**
Complaints cover: Debt collection, Mortgage, Credit card, Credit reporting, Student loan, Bank account, Payday loan, Money transfer, Prepaid card and many more.

**Q: Can I read consumer narratives?**
Yes! Use get_complaints_with_narrative to find complaints that include the consumer's detailed description of their experience.

**Q: How recent is the data?**
The database is updated daily with new complaints. Complaints are published after the company responds or after 15 days, whichever comes first.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cfpb-complaints](https://vinkius.com/mcp/cfpb-complaints)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CFPB Complaints** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cfpb-complaints` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CFPB Complaints** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cfpb-complaints": {
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
