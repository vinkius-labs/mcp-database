# Unstructured MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unstructured)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unstructured-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unstructured-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Process and transform complex unstructured data into AI-ready inputs by managing sources, destinations, and workflows directly from your AI agent.

## Description
Connect your **Unstructured.io** account to any AI agent to automate data ingestion and document processing pipelines seamlessly. Transform complex files into clean, AI-ready data without leaving your workflow.

### What you can do

- **Data Sources** — List all configured remote data connectors (e.g. S3, GCS, SharePoint) to see where documents can be pulled from.
- **Data Destinations** — Browse target locations (like Vector DBs or SQL databases) where structured output is sent.
- **Processing Workflows** — List end-to-end pipelines, retrieve specific workflow configurations, and explore source-destination mappings.
- **Job Execution** — Manually trigger immediate document ingestion and partitioning jobs, and track their execution IDs.
- **Job Monitoring** — List active and historical workflow execution jobs to monitor the progress of your document processing tasks.

### How it works

1. Subscribe to this server
2. Enter your Unstructured API Key and API URL
3. Start managing your data pipelines from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a command center for your entire RAG and knowledge base ingestion pipelines.

### Who is this for?

- **Data Engineers** — troubleshoot and trigger ingestion workflows without opening the Unstructured dashboard.
- **AI Developers** — monitor RAG pipelines and ensure vector databases are populated with clean data directly from code editors.
- **MLOps Teams** — track historical processing jobs and verify that scheduled syncs completed successfully.
- **Product Teams** — quickly audit available sources and destinations when planning new feature integrations.


## Available Tools
- **list_data_sources**: Lists all configured remote data connectors (e.g. S3, GCS)
- **list_data_destinations**: g. Vector DBs, SQL).

Lists all configured target locations for processed data
- **list_processing_workflows**: Lists all end-to-end document processing pipelines
- **get_workflow_details**: Retrieves configuration details for a specific processing workflow
- **trigger_workflow_execution**: Returns a job ID.

Manually triggers an immediate execution of a processing workflow
- **list_workflow_jobs**: Lists all active and historical workflow execution jobs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unstructured** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all our active destination connectors."

**🤖 AI Agent:**
> You have 3 active destinations configured in Unstructured. 
1. Pinecone Index (Production Knowledge Base).
2. MongoDB Atlas Vector Search.
3. AWS S3 (Raw JSON Output). 
Would you like me to check which workflows are currently sending data to the Pinecone index?

---

**👤 You:**
> "List the historical processing jobs from today."

**🤖 AI Agent:**
> I found 2 workflow jobs executed today:
- Job ID `wf_92jdfk`: Completed successfully at 08:30 AM (Ingested 450 PDFs from Sharepoint).
- Job ID `wf_44klqp`: Failed at 11:15 AM (Error connecting to destination Pinecone timeout). 
Would you like me to share more log details about the failed job?

---

**👤 You:**
> "Trigger the engineering onboarding workflow."

**🤖 AI Agent:**
> I have successfully triggered the workflow `wf_eng_onboarding`. The execution has started with Job ID `job_12bxc6`. It is currently processing files from your Google Drive source. Do you want me to monitor it and let you know when it's populated into the Vector DB?


## Installation & Usage

To install and use the **Unstructured** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unstructured](https://vinkius.com/mcp/unstructured)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
