# NYC 311 Service Requests MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nyc-311-service-requests)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [government-public-data](../categories/government-public-data.md)

Keyless 311 service-request queries: search by complaint type, agency, borough, status or date window; look up one request by unique key; top complaint types; counts; and call-center inquiries — no API key.

## Description
311 is New York's non-emergency city-services line: potholes, streetlights, noise, water leaks, rodent complaints, code enforcement. This MCP wraps the live 311 datasets on NYC Open Data — 22M+ service requests since 2020, the historic 2010-2019 set, and the call-center inquiries archive.

### What you can do
- **Search 311 requests** — filter by complaint_type (e.g. "Street Condition"), descriptor, agency code, uppercase borough, status, or a created-date window
- **Look up one request** — by its 10-digit unique key; falls back to the historic dataset automatically
- **Top complaints** — most frequent complaint types in a trailing window (default 7 days) with total volume
- **Count requests** — totals matching any filter combination
- **Call-center inquiries** — information requests and transfers, with how each call was resolved

### Who is this for
Civic reporting, local-government analysis, newsroom verification, and any agent that answers "what is the city's top 311 problem" questions.


## Available Tools (5)
- **count_311_requests**: Use it to size a problem before pulling rows with search_311_requests.

Count 311 service requests with filters
- **get_311_request**: Checks the current dataset (2020+) first, then the historic dataset (2010-2019). Returns the full record including resolution description; says clearly if the key was not found.

Look up one 311 service request by its unique key
- **search_311_inquiries**: The dataset goes back to 2014. inquiry_name is the category (e.g. "Information Request"); rows include the brief description and how the call was resolved.

Search 311 call center inquiries (information requests, not service complaints)
- **search_311_requests**: ). Covers 2020 onward; earlier requests live in a separate historic dataset that get_311_request checks as a fallback. complaint_type values look like "Street Condition" or "Noise"; agency values are short codes (DOT, DOE, NYPD). Borough values are UPPERCASE (MANHATTAN, BROOKLYN, QUEENS, BRONX, STATEN ISLAND). Dates are ISO "YYYY-MM-DD".

Search 311 service requests (noise, potholes, streetlight, ...) with filters
- **top_311_complaints**: Use days to widen or narrow the lookback.

Most frequent 311 complaint types in a recent window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NYC 311 Service Requests** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the top 311 complaints in the last two weeks?"

**🤖 AI Agent:**
> top_311_complaints with days=14 returns the most frequent complaint types in that window plus total request volume.

---

**👤 You:**
> "How many open pothole complaints in Queens?"

**🤖 AI Agent:**
> count_311_requests with complaint_type "Street Condition", descriptor "Pothole", borough "QUEENS", status "Open" returns the total.

---

**👤 You:**
> "Tell me about 311 request 70518024"

**🤖 AI Agent:**
> get_311_request("70518024") returns the full record: complaint type, location, agency, status and resolution.


## ❓ FAQ

**Q: Do I need an API key?**
No. NYC Open Data serves all public datasets anonymously over its SODA API (data.cityofnewyork.us). This MCP defines no credentials and needs nothing configured.

**Q: Borough values differ across datasets — how do I know the format?**
Formats are dataset-specific: 311 and shootings use UPPERCASE ("QUEENS"), food and sanitation use Title Case ("Queens"), DOT potholes use single-letter codes. Tool descriptions state the expected values, and the errors from a mismatched value are reported verbatim by the platform.

**Q: How far back does the 311 data go?**
The main dataset covers 2020 onward (22M+ rows). Requests from 2010-2019 live in the companion historic dataset; get_311_request checks both, so a lookup by unique key works for either era.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nyc-311-service-requests](https://vinkius.com/en/ai-agent-connect/nyc-311-service-requests)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NYC 311 Service Requests** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nyc-311-service-requests` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NYC 311 Service Requests** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nyc-311-service-requests": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
