# Stirling PDF MCP Server

Manage PDF documents via Stirling PDF — add watermarks, convert images to PDF, sign documents with certificates, and monitor server metrics directly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stirling-pdf)

## Overview
**Category:** productivity
**Tools Count:** 11

## Description
Connect your **Stirling PDF** instance to any AI agent and take full control of your document workflows through natural conversation. This server allows you to process PDF files, convert formats, and monitor your self-hosted infrastructure.

### What you can do

- **Document Manipulation** — Add text watermarks with custom opacity and font sizes, or convert images directly into PDF documents.
- **Digital Security** — Sign PDF documents using certificates with specific reasons and location metadata.
- **Server Monitoring** — Track application status, version info, and detailed request metrics (POST/GET) across all endpoints.
- **Advanced Operations** — Use the generic tool runner to access specialized features like merging, splitting, or extracting images from PDFs.
- **Enterprise Metrics** — Access Prometheus metrics for deep observability into your document processing pipeline.

### How it works

1. Subscribe to this server
2. Enter your Stirling PDF Base URL and API Key
3. Start processing documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Automate PDF processing tasks directly from your IDE or terminal.
- **System Administrators** — Monitor the health and load of your Stirling PDF instance in real-time.
- **Legal & Admin Teams** — Quickly sign or watermark documents without leaving your AI chat interface.


## Available Tools
- **add_watermark**: Add a watermark to a PDF document
- **cert_sign**: Sign a PDF document with a certificate
- **get_all_requests**: Get POST requests count for all endpoints
- **get_all_unique_requests**: Get unique users count for all endpoints
- **get_load**: Get total count of GET requests
- **get_prometheus_metrics**: Get Prometheus metrics (requires Enterprise tier)
- **get_requests**: Get total count of POST requests
- **get_status**: Get application status and version information
- **get_unique_requests**: Get count of unique users for POST requests
- **img_to_pdf**: Convert an image to a PDF document
- **run_generic_tool**: Pass additional parameters as a JSON string.

Run any Stirling PDF tool by its ID


## Installation & Usage

To install and use the **Stirling PDF** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stirling-pdf](https://vinkius.com/mcp/stirling-pdf)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
