# Extracta MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/extracta)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [artificial-intelligence](../categories/artificial-intelligence.md)

Automate data extraction via Extracta — process documents into structured JSON, handle AI classification, and audit extraction history directly from any AI agent.

## Description
Connect your **Extracta.ai** account to any AI agent and take full control of your automated data extraction and document classification through natural conversation.

### What you can do

- **Extraction Orchestration** — Create and configure new data extraction processes by defining JSON schemas for fields like dates, amounts, and item descriptions natively
- **Live Document Processing** — Submit publicly accessible file URLs (PDF, JPG, PNG) to trigger asynchronous extraction workflows and retrieve structured JSON data seamlessly
- **AI Classification** — Set up document classification rules to automatically sort documents into types like invoices, receipts, or contracts based on AI predictions
- **Result Auditing** — Retrieve extraction status and finalized structured data for specific documents, evaluating confidence scores and predicted categories flawlessly
- **Batch History Monitoring** — Fetch paginated lists of previously extracted documents and their associated data payloads to track historical processing limitlessly
- **Configuration Mutation** — Update existing extraction settings and mapping rules without creating new endpoints to refine your data parsing logic
- **Workflow Management** — View and manage extraction and classification configurations, including configured fields and webhook settings securely

### How it works

1. Subscribe to this server
2. Enter your Extracta.ai API Key (found in the /api section of your dashboard)
3. Start extracting data from your documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Teams** — automate invoice and receipt processing by extracting structured data using natural language
- **Data Analysts** — convert document-based data into JSON formats for analysis without manual data entry
- **Developers** — test and debug data extraction schemas and verify AI classification results through natural conversation
- **Finance Teams** — audit document extraction history and verify data accuracy in real-time


## Available Tools
- **create_classification**: g. invoice, receipt, contract). Pass JSON schema defining categories.

Create a new Extracta document classification setup
- **view_classification**: View details of an existing document classification process
- **get_batch_results**: Get bulk historical results from an Extraction process
- **get_classification_results**: Get the predicted document category from Extracta
- **create_extraction**: g. language, format, expected fields like invoice_date, total_amount). Returns a new extractionId used for subsequent document processing.

Create a new Extracta.ai data extraction process
- **delete_extraction**: Subsequent uploads to this extractionId will fail.

Delete an Extracta.ai extraction process
- **get_results**: If not completed, it will indicate processing status.

Get extraction results for a specific document
- **update_extraction**: Modifies mapping rules without needing to create a new endpoint.

Update an existing Extracta extraction configuration
- **upload_file_url**: Returns a documentId. Use ea.get_results to poll for extracted data.

Upload a document URL to Extracta for processing
- **view_extraction**: View configuration of an existing Extracta extraction process


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Extracta** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create an extraction process for invoices with fields: date, vendor, total"

**🤖 AI Agent:**
> Extraction setup created! I've initialized a new process (ID: ext_abc) configured to extract 'date', 'vendor', and 'total' fields. You can now start uploading invoice URLs to this process.

---

**👤 You:**
> "Extract data from this receipt URL: https://example.com/receipt.pdf"

**🤖 AI Agent:**
> Processing document... I've submitted the receipt URL for extraction. Document ID: doc_789. I'll poll for the results now... [Agent retrieves structured JSON with date, total, and items].

---

**👤 You:**
> "What type of document is doc_789 according to my classification rules?"

**🤖 AI Agent:**
> Checking classification for doc_789... The AI has classified this document as 'Invoice' with a 98% confidence score. It fits within your defined document categories flawlessly.


## ❓ FAQ

**Q: Can my agent create a new data extraction setup with custom fields?**
Yes. Use the 'create_extraction' tool. Provide a JSON schema defining the fields you expect (e.g., 'total_amount', 'vendor_name'). The agent will return a new extractionId for document processing.

**Q: How do I process a PDF document using a specific extraction ID via chat?**
Use the 'upload_file_url' tool. Provide the extractionId and the public URL of your PDF. The agent will trigger the workflow and return a documentId, which you can use with 'get_results' to fetch the data.

**Q: Can I see the predicted document type and confidence score through the agent?**
Absolutely. Use the 'get_classification_results' tool with the document and classification IDs. The agent will retrieve the AI-predicted label (e.g., 'Invoice') and the confidence score for the processed file.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/extracta](https://vinkius.com/mcp/extracta)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Extracta** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `extracta` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Extracta** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "extracta": {
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
