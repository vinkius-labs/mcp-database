# Cradl AI MCP Server

Equip your AI agent to extract structured data from any document using Cradl AI's deep learning models.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cradl-ai)

## Overview
**Category:** artificial-intelligence
**Tools Count:** 10

## Description
Integrate **Cradl AI**, the advanced document data extraction platform, directly into your AI workflow. Automate the processing of invoices, receipts, IDs, and custom forms using powerful deep learning models and natural language.

### What you can do

- **Data Extraction** — Trigger real-time data extraction from document URLs with high precision.
- **Model Management** — List and explore your custom-trained extraction models.
- **Workflow Monitoring** — Track the status of document processing flows and individual tasks.
- **Batch Processing** — Audit and retrieve details for entire batches of processed documents.

### How it works

1. Connect the Cradl AI integration to your AI assistant.
2. Authorize using your Cradl AI API Key (found in your dashboard).
3. Transform unstructured documents into actionable data via chat.

### Who is this for?

- **Finance Teams** — Automate invoice and receipt processing without manual data entry.
- **Operations Managers** — Monitor high-volume document workflows and extraction accuracy.
- **Developers** — Audit model performance and task statuses during integration testing.


## Available Tools
- **extract_data_from_url**: Touches OCR engine, model prediction, and data normalization boundary.

Trigger a new data extraction prediction from a file URL
- **get_batch_details**: Touches individual file statuses and batch-level processing summary boundaries.

Get details for a specific batch of documents
- **get_flow_details**: Touches integration points and document routing rules boundaries.

Get structure and settings for a specific flow
- **get_model_details**: Touches schema definitions, extraction accuracy metrics, and model metadata boundaries.

Get details for a specific extraction model
- **get_task_status**: Resolves confidence scores and extracted key-value pairs from the document.

Check the status and results of a document task
- **list_batches**: Resolves batch identifiers, creation dates, and total document counts within each batch.

List all document batches
- **list_workflows**: Resolves flow IDs, triggers, and configured processing steps.

List all document processing flows
- **list_extraction_models**: Resolves model names, versions, and training statuses for document analysis.

List all data extraction models in Cradl AI
- **list_processing_tasks**: Resolves task IDs, statuses (PENDING, COMPLETED, FAILED), and processing timestamps.

List recent document processing tasks
- **search_models_by_name**: Resolves model metadata based on a name keyword search.

Search for extraction models by name


## Installation & Usage

To install and use the **Cradl AI** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cradl-ai](https://vinkius.com/mcp/cradl-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
