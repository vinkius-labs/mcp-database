# iLovePDF MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ilovepdf)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Merge, split, compress, and convert PDF files with a complete toolkit that handles every document processing need online.

## Description
Connect your **iLovePDF** account to any AI agent and process PDF documents through natural conversation.

### What you can do

- **Task Management** — Start PDF processing tasks (merge, split, compress, convert) and track progress
- **File Upload** — Upload PDF files by URL for processing
- **Processing** — Execute configured PDF tasks with customizable parameters
- **Download** — Retrieve processed PDF files via download links
- **Status Tracking** — Monitor task completion and get real-time progress updates

### How it works

1. Subscribe to this server
2. Enter your iLovePDF Public Key and Secret Key from the developer portal
3. Start processing PDFs from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Document Teams** — automate PDF merging, splitting, and compression workflows
- **Developers** — integrate PDF processing into AI-powered pipelines
- **Operations** — batch process documents without manual tools


## Available Tools (6)
- **get_pdf_download_link**: Get the processed PDF download link
- **get_task_status**: Check the status of a PDF task
- **list_pdf_tasks**: List recent PDF processing tasks
- **process_pdf_task**: Start processing the PDF
- **start_pdf_task**: g. compress, merge, split). Returns a task ID.

Start a new PDF processing task
- **upload_pdf_by_url**: Upload a PDF file via URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **iLovePDF** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Merge these 3 PDF reports into a single document and compress it."

**🤖 AI Agent:**
> Merge task started (task_4521). Uploading: Q1_Report.pdf ✅, Q2_Report.pdf ✅, Q3_Report.pdf ✅. Processing merge... ✅ Complete! Merged: Combined_Reports.pdf (42 pages, 8.2 MB). Starting compression... ✅ Compressed: 8.2 MB → 2.1 MB (74% reduction). Download ready: Combined_Reports_compressed.pdf. Would you like to split or convert?

---

**👤 You:**
> "Convert the quarterly report PDF to Word format and check all task statuses."

**🤖 AI Agent:**
> Conversion task started (task_4522). Uploading: Q4_Report.pdf ✅. Converting PDF → DOCX... ✅ Complete! Output: Q4_Report.docx (38 pages, preserving formatting). All tasks: task_4521 (merge) — ✅ Completed. task_4522 (convert) — ✅ Completed. task_4519 (compress) — ✅ Completed. 3 tasks completed today.

---

**👤 You:**
> "Split the merged PDF — extract pages 1-10 as a separate document."

**🤖 AI Agent:**
> Split task started (task_4523). Source: Combined_Reports.pdf (42 pages). Extracting pages 1-10... ✅ Complete! Output: Combined_Reports_p1-10.pdf (10 pages, 1.8 MB). Remaining pages available for additional splits. Tasks today: 4 completed (merge, convert, compress, split). Would you like to process another document?


## ❓ FAQ

**Q: Can I merge multiple PDF files into one?**
Yes. Use `start_pdf_task` with task type 'merge', then upload each PDF with `upload_pdf_by_url`, and finally call `process_pdf_task` to execute. Use `get_pdf_download_link` to retrieve the merged result.

**Q: Does iLovePDF require two credentials?**
Yes. iLovePDF uses a **Public Key** and **Secret Key** pair. The server exchanges these for a JWT token automatically via `api.ilovepdf.com/v1`. No manual token management required.

**Q: Can I track the status of a PDF processing task?**
Yes. Use `get_task_status` with the task ID to check progress. Use `list_pdf_tasks` to see all tasks with their current status (pending, processing, completed, failed).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ilovepdf](https://vinkius.com/mcp/ilovepdf)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **iLovePDF** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ilovepdf` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **iLovePDF** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ilovepdf": {
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
