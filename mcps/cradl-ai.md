# Cradl AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cradl-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Equip your AI agent to extract structured data from any document using Cradl AI's deep learning models.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cradl AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract data from this invoice: https://example.com/inv123.pdf using my 'Invoice Parser' model."

**🤖 AI Agent:**
> Extraction started for invoice 'inv123.pdf'. I'll provide the structured data once the 'Invoice Parser' model completes the task. Should I format the results into a table?

---

**👤 You:**
> "Check the status of document processing task 't8s9df7'."

**🤖 AI Agent:**
> Task 't8s9df7' is 100% complete. Cradl AI successfully extracted 15 fields with an average confidence of 98.5%. Would you like to see the extracted JSON?

---

**👤 You:**
> "List all extraction models available in my account."

**🤖 AI Agent:**
> I've found 3 models: 'Invoice Parser', 'ID Document Scanner', and 'Receipt Extractor'. Which one would you like to use for your next document?


## ❓ FAQ

**Q: How do I get a Cradl AI API Key?**
Log in to your Cradl AI dashboard and navigate to the API section to generate a new key. Ensure you keep this key secure.

**Q: Which document formats are supported?**
Cradl AI supports major formats including PDF, JPEG, PNG, and TIFF for data extraction.

**Q: Can I train custom models via chat?**
This integration currently focuses on executing extractions and monitoring tasks. Model training should be performed through the Cradl AI dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cradl-ai](https://vinkius.com/mcp/cradl-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cradl AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cradl-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cradl AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cradl-ai": {
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
