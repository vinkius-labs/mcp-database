# Sensible MCP Server

Extract structured data from PDFs, images, and documents using Sensible's powerful document parsing engine.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sensible)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 37

## Description
Connect **Sensible** to your AI agent to seamlessly extract structured data from unstructured documents like PDFs, Word files, and images.

### What you can do

- **Synchronous Extraction** — Extract data instantly from local documents provided as Base64 strings using `extract_sync` or `extract_sync_with_config`.
- **URL-Based Extraction** — Process documents hosted online asynchronously using `extract_from_url` or `extract_from_url_with_config`.
- **Pre-signed Upload URLs** — Generate secure upload URLs for asynchronous document processing using `generate_upload_url`.

### How it works

1. Subscribe to this server
2. Enter your Sensible API Key
3. Start extracting structured JSON from any document directly from your AI agent

### Who is this for?

- **Developers** — Automate document parsing workflows directly from your IDE or terminal.
- **Operations Teams** — Extract data from invoices, tax forms, and contracts without manual data entry.
- **Data Analysts** — Convert unstructured document repositories into clean, structured datasets.


## Available Tools
- **classify_async**: Classify a document into one of the document types asynchronously
- **classify_sync**: Classify a document into one of the document types synchronously
- **create_configuration**: Create a new configuration for a document type
- **create_document_type**: Create a new document type
- **create_golden**: Create a reference document (Golden). Returns an upload URL
- **delete_configuration**: Delete a configuration
- **delete_configuration_version**: Delete a draft or unpublish a configuration version
- **delete_document_type**: Delete a document type
- **delete_golden**: Delete a reference document
- **extract_from_url_with_config**: Extract data from a document at a URL using a specified config asynchronously
- **extract_from_url**: Extract data from a document at a URL asynchronously
- **extract_portfolio_from_url**: Extract data from a portfolio document at a URL asynchronously
- **extract_sync_with_config**: Extract data from a document using a specified config synchronously
- **extract_sync**: Provide the document as a Base64 string.

Extract data from a document synchronously
- **extract_text_from_golden**: Extract all text lines and positioning coordinates from a reference document
- **generate_csv**: Compile JSON document extractions into a CSV spreadsheet
- **generate_excel**: Compile JSON document extractions into an Excel spreadsheet
- **generate_portfolio_upload_url**: Generate a pre-signed upload URL for portfolio extraction
- **generate_upload_url_with_config**: Generate a pre-signed upload URL for asynchronous extraction using a specified config
- **generate_upload_url**: Generate a pre-signed upload URL for asynchronous extraction
- **get_auth_tokens**: Generates a temporary authorization token for external reviewers
- **get_configuration**: Get a specific configuration
- **get_configuration_version**: Get a specific version of a configuration
- **get_document_type**: Get a specific document type
- **get_document**: Retrieve extraction results by ID
- **get_extraction_statistics**: Returns daily extraction coverage statistics
- **get_golden**: Get reference document metadata
- **list_configuration_versions**: List versions of a configuration
- **list_configurations**: List configurations for a document type
- **list_document_types**: List all document types
- **list_extractions**: Retrieve a filtered, paginated list of past extractions
- **list_goldens**: List reference documents for a document type
- **publish_configuration**: Publish a configuration version to an environment
- **unassociate_golden**: Unassociate a reference document from its configuration
- **update_configuration**: Update a configuration
- **update_document_type**: Update a document type
- **update_golden**: Update reference document metadata


## Installation & Usage

To install and use the **Sensible** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sensible](https://vinkius.com/mcp/sensible)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
