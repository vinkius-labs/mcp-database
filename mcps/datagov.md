# Data.gov MCP Server

Search 300,000+ US government open datasets — agriculture, climate, education, health, finance and more.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/datagov)

## Overview
**Category:** knowledge-management
**Tools Count:** 13

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


## Available Tools
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


## Installation & Usage

To install and use the **Data.gov** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datagov](https://vinkius.com/mcp/datagov)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
