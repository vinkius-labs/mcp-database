# Data.gov MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datagov)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search 300,000+ US government open datasets — agriculture, climate, education, health, finance and more.

## Description
Connect to **Data.gov** and explore the US government's open data catalog through natural conversation — no API key needed.

### What you can do

- **Dataset Search** — Search 300,000+ federal datasets by keyword, organization, tags and topic
- **Dataset Details** — Get full metadata including descriptions, resource downloads, licenses and data dictionaries
- **Browse Organizations** — Explore all federal agencies publishing open data (NASA, USDA, EPA, NOAA, Census Bureau, etc.)
- **Browse by Topic** — Discover datasets organized by topic: agriculture, climate, education, health, finance, public safety
- **Browse by Tags** — Find datasets by popular tags and categories
- **Resource Formats** — Discover available download formats (CSV, JSON, XML, Shapefile, GeoJSON, PDF)

### How it works

1. Subscribe to this server
2. No API key needed — all Data.gov data is public domain
3. Start exploring federal open data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — find federal datasets for academic research and data analysis
- **Journalists** — discover government data for investigative reporting
- **Developers** — integrate federal open data into applications and visualizations
- **Students** — explore real government data for projects and assignments


## Available Tools (13)
- **get_dataset**: gov dataset by its ID or name. Returns full description, organization, tags, resource list (downloadable files), metadata dates, license info and data dictionary.

Get detailed info for a specific dataset
- **get_group**: Returns group name, description, image URL and published datasets (optional). Common groups: "agriculture", "climate", "education", "health", "finance", "public-safety".

Get details for a specific topic group
- **get_organization**: gov. Returns organization name, description, contact info, image URL and published datasets (optional).

Get details for a specific organization
- **get_organization_datasets**: Returns dataset titles, descriptions, resource counts and download links.

Get all datasets published by an organization
- **get_status**: gov API including total counts of datasets, organizations, groups and tags.

Get Data.gov API status and statistics
- **get_tag**: Returns tag name, dataset count and associated datasets (up to 20).

Get details for a specific tag
- **get_tag_datasets**: Returns dataset titles, descriptions, organizations and download links.

Get all datasets with a specific tag
- **get_group_datasets**: Returns dataset titles, descriptions, organizations and download links.

Get all datasets in a specific topic group
- **list_groups**: gov (e.g. agriculture, climate, education, health, finance). Returns group names, descriptions, image URLs and dataset counts.

List all topic groups on Data.gov
- **list_organizations**: gov. Returns organization names, descriptions, dataset counts, logos and contact info.

List all organizations publishing data on Data.gov
- **list_resource_formats**: ). Useful for filtering datasets by preferred format.

List all data formats available in Data.gov resources
- **list_tags**: gov datasets. Returns tag names, dataset counts and display names. Useful for discovering common topics and filtering searches.

List all tags used to categorize datasets
- **search_datasets**: gov catalog of US federal government open datasets. Supports free-text search and filtering by organization, tags, groups. Returns dataset titles, descriptions, organizations, resource counts, tags and download links. Sort options include "metadata_modified desc" (recent), "views_recent desc" (popular).

Search US government open data datasets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Data.gov** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for climate change datasets."

**🤖 AI Agent:**
> Found 5,000+ climate-related datasets including: NOAA Climate Data, NASA GISS Surface Temperature, EPA Greenhouse Gas Emissions, Census Climate Vulnerability and many more.

---

**👤 You:**
> "What datasets does NASA publish?"

**🤖 AI Agent:**
> NASA publishes 2,000+ datasets including: Earth Observations, Climate Data, Asteroid/Comet Catalogs, Satellite Imagery, Solar Activity, Exoplanet Data and many more.

---

**👤 You:**
> "Find education datasets about student performance."

**🤖 AI Agent:**
> Found 800+ education datasets including: NAEP Student Assessment, College Scorecard, Civil Rights Data Collection, Education Spending and many more from Department of Education.


## ❓ FAQ

**Q: Do I need an API key?**
No! Data.gov data is public domain and freely accessible. No authentication required.

**Q: How many datasets are available?**
Data.gov catalogs 300,000+ datasets from over 200 federal agencies including NASA, USDA, EPA, NOAA, Department of Education, Census Bureau and many more.

**Q: What organizations publish data?**
Over 200 federal agencies including NASA, USDA, EPA, NOAA, Department of Education, Census Bureau, Department of Transportation, FBI, CDC, FDA and many more.

**Q: What formats are available?**
Common formats: CSV, JSON, XML, Shapefile, GeoJSON, PDF, HTML, RDF, KML, ZIP. Use list_resource_formats to see all available formats.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datagov](https://vinkius.com/mcp/datagov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Data.gov** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `datagov` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Data.gov** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "datagov": {
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
