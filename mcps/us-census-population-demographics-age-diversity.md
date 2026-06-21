# U.S. Census Population — Demographics, Age & Diversity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-census-population-demographics-age-diversity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access demographic data from the American Community Survey (ACS). Get total population, median age, and detailed racial/ethnic breakdowns (White, Black, Asian, Hispanic, Foreign-born) for any U.S. state, county, or city.

## Description
U.S. Census demographic data.

### 5 Tools
- **State Population** — View 50 states + DC
- **County Population** — Drill down into counties
- **City/Place Population** — Get local data
- **State Demographics** — Race and ethnicity by state
- **County Demographics** — Race and ethnicity by county

### Authentication
Requires a free API key from the Census Bureau.


## Available Tools
- **get_population_by_state**: The ACS is the most comprehensive demographic survey in the U.S., sampling 3.5 million households annually.

Get total population and median age for all 50 U.S. states + DC
- **get_population_by_county**: Use state FIPS codes: CA=06, TX=48, NY=36, FL=12, IL=17, PA=42, OH=39, GA=13, NC=37, MI=26, etc.

Get population and median age for all counties in a state
- **get_population_by_city**: This includes incorporated cities and Census Designated Places.

Get population for all cities/towns/places within a state
- **get_demographics_by_state**: Essential for diversity analysis, market segmentation, and policy research.

Get racial and ethnic demographics for all states — White, Black, Asian, Hispanic, foreign-born
- **get_demographics_by_county**: Get racial and ethnic demographics for all counties in a state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Census Population — Demographics, Age & Diversity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the population and median age of California vs Texas?"

**🤖 AI Agent:**
> 📊 **U.S. Census Bureau: Population by State**

**California (06):**
- Population: 39,040,616
- Median Age: 37.8 years

**Texas (48):**
- Population: 29,730,311
- Median Age: 35.4 years

---

**👤 You:**
> "Show the Hispanic and Asian population for Florida"

**🤖 AI Agent:**
> 📊 **Demographics by State**

**Florida (12):**
- Total Population: 22,244,823
- Hispanic or Latino: 5,956,878 (26.8%)
- Asian Alone: 668,744 (3.0%)

---

**👤 You:**
> "What is the most populated county in New York State?"

**🤖 AI Agent:**
> 📊 **Population by County — State 36**

The most populated county is:
**Kings County (Brooklyn) (36-047)**
- Population: 2,590,516
- Median Age: 35.8

Followed by:
**Queens County (36-081)**
- Population: 2,278,029


## ❓ FAQ

**Q: What are FIPS codes?**
FIPS (Federal Information Processing Standard) codes are numbers used by the government to uniquely identify states, counties, and places. E.g., California is 06, Los Angeles County is 037.

**Q: Which census survey do you use?**
We use the American Community Survey (ACS) 5-Year estimates, which provide the most reliable, detailed, and broad demographic data annually.

**Q: Are undocumented immigrants counted?**
Yes, the Census Bureau attempts to count all residents regardless of immigration status, though this group is historically harder to count accurately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-census-population-demographics-age-diversity](https://vinkius.com/mcp/us-census-population-demographics-age-diversity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **U.S. Census Population — Demographics, Age & Diversity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-census-population-demographics-age-diversity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **U.S. Census Population — Demographics, Age & Diversity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-census-population-demographics-age-diversity": {
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
