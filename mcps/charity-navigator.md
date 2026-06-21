# Charity Navigator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/charity-navigator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Search and evaluate US nonprofits — get charity ratings, financial health, advisories and cause data from any AI agent.

## Description
Connect to **Charity Navigator** and access ratings for over 175,000 US nonprofits through natural conversation.

### What you can do

- **Charity Search** — Search nonprofits by name, keyword, location, cause area or rating
- **Ratings** — Get Charity Navigator's overall rating (0-4 stars) plus financial health and accountability scores
- **Organization Details** — View mission statements, financials, website, contact info and tax filings
- **Rating History** — See how a charity's rating has changed over time
- **Advisories** — Check for warnings and alerts about charities with governance or financial concerns
- **Categories** — Browse charity categories and causes (education, health, environment, animal welfare, etc.)

### How it works

1. Subscribe to this server
2. Enter your Charity Navigator App ID and App Key (free registration)
3. Start evaluating charities from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Donors** — research charities before donating and verify their financial health
- **Researchers** — explore nonprofit ratings, financial data and governance records
- **Philanthropists** — search by cause area, location and rating to find vetted organizations


## Available Tools
- **get_all_advisories**: Useful for identifying charities with governance, financial or operational concerns.

Get all organizations with active advisories
- **get_categories**: Each category includes its ID, name, parent category and description. Use category IDs to filter charity searches by cause area (e.g. education, health, environment, animal welfare).

Get all charity categories and causes
- **get_charity**: Returns the charity name, EIN, mission statement, website, address, phone, financial data, tax filings and contact info. Use search_charities to find EINs.

Get detailed info for a specific charity by EIN
- **get_charity_advisories**: Advisories may include issues with financial management, governance or fundraising practices. Optionally filter by status (ALL, ACTIVE, REMOVED).

Get advisories/warnings for a specific charity
- **get_charity_ratings**: Returns all historical Charity Navigator ratings with overall score, financial health, accountability, transparency and impact scores. Shows how the charity's rating has changed over time.

Get rating history for a specific charity
- **search_charities**: Supports powerful filters: free-text search, state, city, zip code, rating (0-4 scale), category/cause, organization size by expenses, and whether the org is rated. Sort by rating, name or relevance. Pagination with pageSize (max 1000) and pageNum (max 10). Returns charity names, EIN, mission, ratings and financial info.

Search for charities and nonprofits by name, location or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Charity Navigator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the top-rated education charities in California."

**🤖 AI Agent:**
> Found 50+ education charities in California with 4-star ratings. Top results include: DonorsChoose (EIN: 13-4125734, 4/4 stars, $100M+ expenses), First Book (EIN: 52-1760363, 4/4 stars), and Room to Read (EIN: 94-3384184, 4/4 stars). All rated exceptional for financial health and accountability.

---

**👤 You:**
> "Show me the rating history for the American Red Cross."

**🤖 AI Agent:**
> American Red Cross (EIN: 53-0196605): Current rating 3/4 stars. Historical ratings show consistent 3-4 star performance over the past decade. Financial health: Good. Accountability & transparency: Strong. Total expenses: $3.2B annually.

---

**👤 You:**
> "Are there any advisories for charities named 'Red Cross'?"

**🤖 AI Agent:**
> No active advisories found for American Red Cross (EIN: 53-0196605). The organization has a clean record with no warnings or flags from Charity Navigator.


## ❓ FAQ

**Q: How do I get Charity Navigator API credentials?**
Visit [**charitynavigator.org**](https://www.charitynavigator.org/index.cfm?bay=content.view&cpid=6322), register for a free developer account, and you'll receive an App ID and App Key. Both are required for API access.

**Q: What does the rating scale mean?**
Charity Navigator rates nonprofits on a 0-4 star scale. 4 stars = exceptional performance, 3 stars = strong, 2 stars = adequate, 1 star = needs improvement, 0 = unrated or flagged. Ratings are based on financial health, accountability and transparency.

**Q: How do I search for charities by cause?**
Use get_categories to get all cause/category IDs, then use search_charities with the category_id parameter. Popular categories include education, health, environment, animal welfare, arts & culture, and human services.

**Q: What is an EIN?**
EIN stands for Employer Identification Number, a unique 9-digit identifier assigned by the IRS to US nonprofits. It's used as the primary key for looking up specific charities. You can find EINs in search results or on the charity's tax filings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/charity-navigator](https://vinkius.com/mcp/charity-navigator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Charity Navigator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `charity-navigator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Charity Navigator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "charity-navigator": {
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
