# Zamzar MCP Server

Convert files between 1100+ formats — transform documents, images, videos, and audio directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zamzar)

## Overview
**Category:** productivity
**Tools Count:** 5

## Description
Connect your **Zamzar** developer account to any AI agent and automate complex file conversion workflows using natural language. Zamzar supports over 1100 formats including PDF, DOCX, PNG, MP4, and more.

### What you can do

- **Format Discovery** — Use `list_formats` to see all supported conversions or `get_format` to check specific target options and credit costs.
- **File Conversion** — Trigger `start_job` to convert files from any public URL or S3 URI to your desired output format.
- **Status Monitoring** — Track the progress of your conversions with `get_job`, monitoring states from initialising to successful.
- **Content Retrieval** — Once a conversion is finished, use `get_file_content` to download the binary data of your new file.

### How it works

1. Subscribe to this server
2. Enter your Zamzar API Key
3. Start converting files directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Quickly convert images or videos to web-ready formats without leaving your workflow.
- **Developers** — Automate document processing and file transformations within your coding environment.
- **Business Professionals** — Instantly turn PDFs into editable documents or spreadsheets via simple chat commands.


## Available Tools
- **get_file_content**: Returns metadata about the downloaded file.

Download the converted file content
- **get_format**: Retrieve details for a specific format
- **get_job**: Statuses include initialising, converting, successful, failed.

Retrieve the status of a specific job
- **list_formats**: List all supported file formats
- **start_job**: Start a file conversion job


## Installation & Usage

To install and use the **Zamzar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zamzar](https://vinkius.com/mcp/zamzar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
